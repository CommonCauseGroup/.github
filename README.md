<div align="center">

# `.github`

**The public face of the Common Cause organisation on GitHub.**

<img alt="Visibility" src="https://img.shields.io/badge/visibility-public-3dbcc9?style=flat-square">
<img alt="Provides" src="https://img.shields.io/badge/provides-org%20defaults-5b3bbd?style=flat-square">
<img alt="Issue forms" src="https://img.shields.io/badge/issue%20forms-4-4c6fd6?style=flat-square">

<br>

**[See the organisation page →](https://github.com/CommonCauseGroup)**

</div>

---

This repository holds two different things, and GitHub treats them differently.

## What is in here

| Path | What GitHub does with it |
| --- | --- |
| **[`profile/README.md`](profile/README.md)** | Rendered on **[the organisation's public page](https://github.com/CommonCauseGroup)**. Anyone can see it, signed in or not. |
| **[`CONTRIBUTING.md`](CONTRIBUTING.md)** · **[`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md)** · **[`SECURITY.md`](SECURITY.md)** · **[`SUPPORT.md`](SUPPORT.md)** | **Default community health files.** Every public repository in the organisation without its own copy inherits these — they appear in its sidebar, its new-issue page and its Security tab without being committed there. |
| **[`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE)** | The default issue forms — bug, idea, documentation, accessibility — and the links shown above them. Inherited the same way. |
| **[`.github/PULL_REQUEST_TEMPLATE.md`](.github/PULL_REQUEST_TEMPLATE.md)** | The default pull request description. Inherited the same way. |
| **[`.github/brand/`](.github/brand)** | The horizontal lockup, full colour and the `-white` cut, for the profile page. A committed copy rather than a symlink — GitHub does not follow a symlink when rendering an image. |

> [!IMPORTANT]
> **A repository's own copy always wins.** Put a file here for the answer that
> is true across the organisation; put it in the repository itself when that
> repository needs a different one — a library with its own supported-versions
> policy, say. **Deleting a file here silently removes it from every repository
> relying on it**, so check before you do.

`profile/README.md` is the only file the organisation page shows. This file is
not displayed there, which is why it can be a note to ourselves rather than a
front page.

<br>

## Before this goes public

<details open>
<summary><b>Placeholders and settings still to sort out.</b> The documents carry <code>&lt;our domain&gt;</code> and <code>&lt;our support address&gt;</code>, spelt that way so they are obvious in rendered Markdown. Delete this section once it is done.</summary>

<br>

> [!CAUTION]
> **Confirm the crisis routes first.** [`SUPPORT.md`](SUPPORT.md),
> [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) and
> [`profile/README.md`](profile/README.md) currently name UK services — **999**,
> Samaritans on **116 123**, Shout on **85258**, NHS **111** — plus
> [findahelpline.com](https://findahelpline.com) for everywhere else. If we
> operate anywhere other than the UK these need a second look from somebody
> clinical, not from engineering. **Getting these wrong is the worst mistake
> this repository can make**, so nothing else on this list matters more.

**Addresses**

- [ ] `security@<our domain>` — in [`SECURITY.md`](SECURITY.md) (three times) and [`CONTRIBUTING.md`](CONTRIBUTING.md)
- [ ] `conduct@<our domain>` — in [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md)
- [ ] `<our support address>` — in [`SUPPORT.md`](SUPPORT.md)
- [ ] Link the API documentation from [`SUPPORT.md`](SUPPORT.md) § 3 once it has a public address

**Organisation settings the documents assume**

- [ ] **Turn on Discussions**, or remove the three links to `/orgs/CommonCauseGroup/discussions` — in [`CONTRIBUTING.md`](CONTRIBUTING.md), [`SUPPORT.md`](SUPPORT.md) and [`.github/ISSUE_TEMPLATE/config.yml`](.github/ISSUE_TEMPLATE/config.yml)
- [ ] **Turn on private vulnerability reporting** for every public repository — organisation settings → Code security. [`SECURITY.md`](SECURITY.md) tells people to use it, and without it the button it names is not there
- [ ] **Create the labels the issue forms apply**: `bug`, `enhancement`, `documentation`, `accessibility`, `needs triage` — plus `good first issue` and `help wanted`, which [`profile/README.md`](profile/README.md) points newcomers at
- [ ] **Check every public repository has a `LICENSE`**, since [`profile/README.md`](profile/README.md) and [`CONTRIBUTING.md`](CONTRIBUTING.md) both send contributors to it

**Promises**

- [ ] Confirm the response times we commit to are ones we will meet: **5 working days** for issues and pull requests, **2** for security reports, **3** for conduct reports, **10** for a security assessment, **90 days** to disclosure. A promise we miss is worse than a longer one we keep.

</details>

<br>

## Changing these files

They are read by people we have never met, at the moment they have a problem.
Two habits keep them worth reading:

**Say the specific thing.** "We aim to respond promptly" tells a reader nothing;
"within five working days" tells them whether to wait or chase.

**Keep the language rules we ask of contributors.** [`CONTRIBUTING.md` § Language
about people](CONTRIBUTING.md#language-about-people) applies to
`CONTRIBUTING.md`. The full version of those rules — and the reasoning behind
each — lives in `group/brand/BRAND.md` § 5 in the estate; this is its public,
shorter half, and the two should not drift.

<br>

## The private counterpart

**[`CommonCauseGroup/.github-private`](https://github.com/CommonCauseGroup/.github-private)**
holds the staff handbook and the members-only organisation profile. It is
visible only to members, and nothing from it belongs here.
