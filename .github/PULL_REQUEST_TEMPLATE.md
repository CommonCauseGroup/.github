<!--
Thank you. Filling this in properly is the difference between a review this
week and a conversation over three.

Anything genuinely not applicable: write "n/a" rather than deleting the
heading, so a reviewer can tell you considered it.
-->

## What this changes

<!-- One or two sentences in plain language. What is different afterwards? -->

## Why

<!--
The problem, not the patch. If there is an issue, link it: "Closes #123".
If there is no issue and this is more than a fix, say why it did not need one.
-->

## How it works

<!--
Only the part a reviewer could not work out from the diff: the approach you
chose, what you decided against, and anything that looks odd but is deliberate.
This is the most valuable section in the form — a note here saves a round trip.
-->

## How you tested it

<!--
Which tests you added and what they pin. If you could not add one, say what you
did by hand instead, step by step.
-->

- [ ] There is a test that fails before this change and passes after it
- [ ] The existing suite passes locally

---

## Checks

- [ ] **One change.** No unrelated renames, reformatting or drive-by fixes bundled in.
- [ ] **British English**, in identifiers and comments as well as in copy — `organisation`, `licence`, `colour`.
- [ ] **Person-first, plain language** in anything a person will read. No "just", no "committed suicide", no urgency the software cannot honour. See [CONTRIBUTING.md](https://github.com/CommonCauseGroup/.github/blob/main/CONTRIBUTING.md#language-about-people).
- [ ] **No new call to a domain we do not own** — fonts, analytics, CDNs, error trackers — or it is called out below and was agreed in the issue first.
- [ ] **No new logging of request bodies, identifiers in URLs, or anything typed into a form.**
- [ ] **No secrets, keys, tokens or real people's data** in the diff, the fixtures, the tests or the screenshots.
- [ ] Any new dependency is named below with what it does and why nothing we already have would do.

### If this touches the interface

- [ ] Works with a keyboard alone, and the focus order makes sense
- [ ] Correct in **dark mode** as well as light — dark is the scheme these interfaces are designed in
- [ ] Readable at 200% zoom and on a narrow screen
- [ ] Contrast meets WCAG AA without lowering a design token
- [ ] Screenshots below, both schemes, if anything visible changed

### If this changes an API or the database

- [ ] Existing integrations still work, or the break is described below and deliberate
- [ ] The migration is safe to run against live data, and reversible or explicitly not
- [ ] Documentation updated in the same pull request

## Anything a reviewer should know

<!--
New dependencies. Things you are unsure about. A follow-up you have deliberately
left out of scope. Somewhere you would like a second opinion.

Saying "I am not sure about the approach in X" is not a weakness in a pull
request — it is the fastest route to a useful review.
-->
