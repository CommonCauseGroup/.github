# Security policy

We run identity and health-adjacent systems. A vulnerability here is not an
inconvenience — it is somebody's mental health record, or the sign-in that
guards it. We would much rather hear from you than not.

## Reporting a vulnerability

**Do not open a public issue.** A public report is a working exploit with an
audience.

Use one of these, in order of preference:

1. **GitHub private vulnerability reporting** — the *Report a vulnerability* button under the **Security** tab of the affected repository. This gets it to us fastest, keeps the whole thread private, and gives you credit automatically if a advisory is published.
2. **Email security@\<our domain\>.** Encrypt it if you like; if you need a key, ask in a first message with no details in it.

**Do not include real people's data.** If your finding involves a live account,
describe how to reach it — do not paste what you found. If you have already
retrieved personal data, say so, and delete your copy.

### What to send

Whatever you have. A rough report of a real problem beats a polished report of
a theoretical one. If you can, include:

- Which repository, host or product, and roughly when you tested.
- What an attacker gets — read another person's data, act as them, escalate, deny service.
- The steps, precisely enough that we can reproduce it. A curl command is perfect.
- Anything that limits it: needs an authenticated session, needs to be on the same network, needs a specific configuration.

### What we promise

| | |
| --- | --- |
| **Acknowledgement** | Within **2 working days**, from a person, not a bot. |
| **First assessment** | Within **10 working days** — whether we agree it is a vulnerability, how severe we think it is, and what happens next. |
| **Progress** | An update at least every **10 working days** until it is closed. |
| **Fix** | Critical and high issues are worked on immediately. Others are scheduled and we tell you the schedule. |
| **Credit** | Named in the advisory and the release notes, however you would like to be named — or not at all, if you would rather. |
| **Good faith** | If you follow this policy, we will not pursue or support legal action against you for your research, and we will say so publicly if anyone else does. |

We do not run a paid bug bounty. We will say thank you properly, and we will
mean it.

## Scope

**In scope:** every public repository in this organisation; the Common Cause
products and their APIs; our sign-in and any host under a domain we operate.

**Out of scope** — please do not spend your time on these, and we will close
reports about them:

- Anything requiring physical access to somebody's unlocked device.
- Social engineering of our staff, our customers, or their patients. This is a hard line for us: **do not contact a person using one of our services as part of your research**, under any pretext.
- Denial of service, volumetric testing, and anything that degrades a live system. If you believe you have found a DoS, describe it — do not demonstrate it.
- Reports produced only by a scanner, with no demonstrated impact.
- Missing hardening headers, cookie flags on non-session cookies, weak TLS ciphers, and similar, without a working attack behind them.
- Self-XSS, clickjacking on pages that do not change state, and username enumeration on a signup form that is public by design.
- Third-party services we merely use. Report those to them; tell us too, and we will help chase it.

### Testing safely

Use accounts you created. If a test needs two accounts, create two. Stop at the
point you have proved the issue — one record is proof, a thousand is a breach.

## When it is somebody else's data, not a bug

If you have come across Common Cause data somewhere it should not be — in a
public bucket, in a paste, in a search result — that is not a vulnerability
report, it is more urgent than one. Email **security@\<our domain\>** with the
location and nothing else. Do not download it to check.

## Supported versions

We support the current release of each product. These repositories are the
source for hosted services rather than software you install and run, so an old
tag is a historical record, not a supported version. Where a repository ships a
library that others install, that repository's own `SECURITY.md` states its
supported versions and overrides this file.

## Disclosure

We work to **coordinated disclosure**. We will agree a date with you; our
default is to publish a GitHub Security Advisory once a fix is deployed, and
within **90 days** of your report regardless — if we cannot fix something in 90
days, that is a fact worth publishing too.

If a vulnerability is being actively exploited, we will move immediately and
tell you what we did afterwards.
