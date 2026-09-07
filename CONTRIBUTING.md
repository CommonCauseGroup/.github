# Contributing to Common Cause

Thank you for being here. This file is the whole deal: what we will merge, what
we will ask you to change, and how long each step takes. It applies to every
public repository in the `CommonCauseGroup` organisation unless that repository
has its own `CONTRIBUTING.md`, which then wins.

Read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) as well. It is short and it is
enforced.

---

## Before you write any code

**Open an issue first for anything that is not a bug fix.** Not as a formality —
we would rather tell you in a paragraph that a feature is already half-built on
a branch than have you find out from a closed pull request. For a typo, a broken
link, or a clearly wrong line, skip straight to the pull request.

**Say what problem you are solving, not what code you want to add.** The best
issue we get says: here is what I was trying to do, here is what happened, here
is what I expected. What the fix should be is often the part we can help with.

**Do not send us other people's data.** Logs, screenshots, database dumps and
`.har` files from a real deployment routinely contain names, email addresses and
session tokens. Redact before you paste. If you have already posted something
you should not have, email **security@\<our domain\>** and we will remove it —
you will not be in trouble for telling us.

## The change itself

**One change per pull request.** A rename bundled with a bug fix means the fix
cannot be reverted without the rename, and it will get a slower review from a
more nervous reviewer.

**Match the code around you.** Every repository here has an accent — how much it
comments, how it names things, how it structures a test. Read the neighbouring
file before deciding what "idiomatic" means; consistency with the file beats
consistency with your own habits.

**British English, in the code as well as the copy.** `organisation`,
`licence`, `colour`, `behaviour`, `authorised`. This is not a preference we are
willing to have half of: a codebase with `color` in one model and `colour` in
the next costs everybody a lookup every time.

**Write comments that say why.** A comment restating the line above it is noise;
a comment naming the failure mode that made the code look like this is the most
valuable thing in the file. If you worked something out the hard way, leave it
written down — that is a contribution on its own.

### Language about people

This is not a style nicety here, it is the product. Our software is used by
people having the worst year of their life, and every string in it was written
by somebody in a hurry.

- **Person first.** "A person with schizophrenia", not "a schizophrenic". "A person using the service", not "a service user", wherever it can be avoided.
- **Never "committed suicide."** "Died by suicide", or "took their own life". *Committed* belongs to crimes and to sins.
- **No "suffering from", no "battling", and no "survivor" applied to somebody who did not choose the word.** Say what happened.
- **Never "just".** Not "just click here", not "just talk to somebody". It makes a hard thing sound easy and the reader feel stupid for finding it hard.
- **Promise no urgency the software can honour.** Do not put "get help now" above a form with a fourteen-day wait. Say what the wait is.
- **Crisis information is plain, first, and never behind a click.** It does not get a gradient, a modal, or a marketing tone.

These apply to variable names, table columns, enum cases, commit messages, test
fixtures and comments — not only to user-visible strings. Reviewers will ask for
changes on this, and we would rather flag it kindly at review than have it ship.

### Privacy, and what a new dependency costs

The fact that somebody loaded one of our pages is information about their mental
health. That single sentence decides a lot of arguments before they start.

- **A new network call to a domain we do not own is a design decision.** Fonts, analytics, error trackers, CDN-hosted libraries, avatar services. Raise it in the issue, not in the pull request — the answer is sometimes yes, but never quick.
- **Do not add logging that captures request bodies, URLs with identifiers in them, or anything typed into a form.**
- **New dependencies need a reason in the pull request description**: what it does, why the standard library or an existing dependency will not, and roughly what it drags in.

### Accessibility

Every user-facing change is expected to work with a keyboard, be usable at 200%
zoom, and survive a screen reader. Dark mode is not an afterthought here — it is
the scheme the interfaces are designed in, and a change that only looks right in
light mode is unfinished. Contrast is checked against WCAG AA; do not lower a
token to make a design work.

### Tests

Add a test that fails before your change and passes after it. If you genuinely
cannot — a build script, a layout tweak — say so in the description and say how
you checked it by hand instead.

The test we value most is the one that pins the thing that was *surprising*:
the argument that silently gets dropped, the header without which the whole
route 500s, the flag that means two different things. A test named for the
mistake is worth five that assert the obvious.

## Sending it

1. **Fork, then branch.** Name the branch for the change — `fix/expired-invite-500`, not `patch-1`.
2. **Commit in the imperative present**: "Reject an invitation whose licence has lapsed". A commit message body explaining *why* is welcome and often better than the diff.
3. **Fill in the pull request template.** The fields are there because reviewers ask those questions every time.
4. **Push, open the pull request, and let CI finish** before asking for a review — a red build is the answer to most first-round questions anyway.
5. **Sign off that the work is yours to give.** By opening a pull request you confirm you wrote the change, or have the right to contribute it, and that it may be released under the licence of the repository you are contributing to. See that repository's `LICENSE` file — the licence differs between our repositories, and some of them are not open source at all.

### What review looks like

A maintainer will look at it, and the first response will be within **five
working days**. It will be one of: merged, a set of questions, or an honest no
with the reason. We try hard not to leave pull requests sitting silently; if
yours has gone quiet for longer than that, a nudge in the thread is welcome and
not rude.

We will be direct about the code and kind about you. If a review of ours ever
reads otherwise, that is a bug in the review, and telling us so is fine.

**Reasons we say no**, so none of them are a surprise: the change is a good idea
in the wrong repository; it adds a dependency or a third-party call whose cost
we are not willing to pay; it makes something configurable that we want to keep
having one answer; or it is a feature we have deliberately decided against, in
which case we will say why and link to where that was decided.

## Running things locally

Each repository's own `README.md` is the authority on getting it running — how
to install it, what it needs, and how to run its tests. Where several of our
applications have to talk to each other to be worth running at all, that
repository's README says so and says what to do about it.

If the README is wrong, out of date, or assumes something it did not tell you,
**that is a bug worth reporting.** It is also one of the most useful pull
requests we receive, because the person who just hit the problem is the only one
who can still see it.

## Anything else

Open a **[discussion](https://github.com/orgs/CommonCauseGroup/discussions)** if
there is one, or ask in the issue. Questions are not an imposition — an
unanswered question usually means our documentation failed, which is our problem
and not yours.
