# `.github`

This repository is the **public** face of the `CommonCauseGroup` organisation on
GitHub. It holds two different things, and GitHub treats them differently.

## What is in here

| Path | What GitHub does with it |
| --- | --- |
| `profile/README.md` | Rendered on **[the organisation's public page](https://github.com/CommonCauseGroup)**. Anyone can see it, signed in or not. |
| `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `SUPPORT.md` | **Default community health files.** Every public repository in the organisation that does not have its own copy inherits these — they appear in its sidebar, its new-issue page and its Security tab without being committed there. |
| `.github/ISSUE_TEMPLATE/` | The default issue forms, and the links shown above them. Inherited the same way. |
| `.github/PULL_REQUEST_TEMPLATE.md` | The default pull request description. Inherited the same way. |

**A repository's own copy always wins.** Put a file here for the answer that is
true across the organisation; put it in the repository itself when that
repository needs a different one — a library with its own supported-versions
policy, say. Deleting a file here silently removes it from every repository that
was relying on it, so check before you do.

`profile/README.md` is the only file the organisation page shows. This file —
the root `README.md` — is not displayed there, which is why it can be a note to
ourselves rather than a front page.

## Before this goes public

These are the placeholders the documents carry, spelt `<our domain>` and
`<our support address>` so they are obvious in rendered Markdown. Replace all of
them, then delete this section.

- [ ] `security@<our domain>` — in `SECURITY.md` (three times), `CONTRIBUTING.md`
- [ ] `conduct@<our domain>` — in `CODE_OF_CONDUCT.md`
- [ ] `<our support address>` — in `SUPPORT.md`
- [ ] **Confirm the crisis routes** in `SUPPORT.md`, `CODE_OF_CONDUCT.md` and `profile/README.md`. They currently name UK services — 999, Samaritans on 116 123, Shout on 85258, NHS 111 — plus findahelpline.com for everywhere else. If we operate anywhere other than the UK, these need a second look from somebody clinical, not from engineering. **Getting these wrong is the worst mistake this repository can make**, so nothing else on this list matters more.
- [ ] Link the API documentation from `SUPPORT.md` § 3 once it has a public address
- [ ] **Turn on Discussions for the organisation**, or remove the three links to `/orgs/CommonCauseGroup/discussions` (in `profile/README.md`, `CONTRIBUTING.md`, `SUPPORT.md` and `.github/ISSUE_TEMPLATE/config.yml`)
- [ ] **Turn on private vulnerability reporting** for every public repository — organisation settings → Code security. `SECURITY.md` tells people to use it, and without it the button it names is not there
- [ ] Create the labels the issue forms apply: `bug`, `enhancement`, `documentation`, `accessibility`, `needs triage` — plus `good first issue` and `help wanted`, which `profile/README.md` points newcomers at
- [ ] Check the response times we commit to are ones we will meet: **5 working days** for issues and pull requests, **2** for security reports, **3** for conduct reports, **10** for a security assessment. A promise we miss is worse than a longer one we keep

## Changing these files

They are read by people we have never met, at the point they have a problem.
Two habits keep them worth reading:

**Say the specific thing.** "We aim to respond promptly" tells a reader
nothing; "within five working days" tells them whether to wait or chase.

**Keep the language rules we ask of contributors.** `CONTRIBUTING.md` § *Language
about people* applies to `CONTRIBUTING.md`. The full version of those rules —
and the reasoning behind each one — lives in `group/brand/BRAND.md` § 5 in the
estate repository; this file is its public, shorter half, and the two should not
drift.

The staff-facing counterpart to this repository is
[`.github-private`](https://github.com/CommonCauseGroup/.github-private), which
holds the handbook and is visible only to members of the organisation.
