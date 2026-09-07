# Getting help

There are four different problems people arrive here with, and only one of them
belongs on GitHub. This page is the map.

---

## 1. You are struggling, or worried about somebody

**Please do not use GitHub for this.** Nobody is watching it out of hours, an
issue can sit for days, and everything filed here is public and permanent.

If you are in immediate danger, call **999** (UK) or your local emergency
number.

To talk to somebody, any hour of any day:

| | |
| --- | --- |
| **Samaritans** | **116 123** — free, from any phone, 24 hours. Or email `jo@samaritans.org`. |
| **Shout** | Text **SHOUT** to **85258** — free, 24 hours, if a conversation by text is easier than one out loud. |
| **NHS 111** | **111**, option 2, for urgent mental health help in England. |
| **Outside the UK** | [findahelpline.com](https://findahelpline.com) will find the service where you are. |

You do not have to be in crisis to call any of them. "I am not sure this counts"
is a normal way to start.

---

## 2. Something is wrong with your account or one of our products

Sign-in that will not work, a licence that looks wrong, a charge you did not
expect, data you want a copy of or deleted — that is our support team, not this
repository. They can see your account; GitHub maintainers cannot, and should
not.

**Contact support at \<our support address\>.**

Please do not post account details, invoices, screenshots of your inbox or
anything with your name in it into a GitHub issue. Once it is in a public
repository it is in search results, in forks and in archives, and we cannot
fully take it back.

**A note on how our support works, because it surprises people:** an agent can
put a prompt on your screen asking to open your account, and it shows a
six-digit code. **We will never ask you to read that code to us, and we will
never ask for your password or a sign-in code.** The code is there for *you* to
check against what the agent is telling you, so you know the prompt is theirs
and not somebody else's. If anyone asks you to read it out, that is not us —
hang up and tell support.

---

## 3. You are building against our API

- **The documentation** is the first stop, and if it did not answer your question that is a documentation bug worth telling us about.
- **[Discussions](https://github.com/orgs/CommonCauseGroup/discussions)** for "how do I", "is this supposed to", and "am I holding this wrong". Ask in public if you can — the next person searching for it will find your thread.
- **An issue on the relevant repository** once you are fairly sure the behaviour is a bug, with a request and a response, minus your key.

**Never paste an API key, an access token, or an `Authorization` header into an
issue.** If you already have, revoke the key in the console first and then tell
us — the revocation is the fix; deleting the comment is not, because it is in
the edit history and in anyone's notification email.

---

## 4. You have found a bug in our code, or want to change it

You are in the right place.

- **[Contributing](CONTRIBUTING.md)** — how to send a change, what review is like, and what we will ask you to fix.
- **A bug report** — open an issue on the repository it belongs to. If you are not sure which, open it anywhere and say so; moving an issue is one click for us.
- **A security vulnerability** — **[SECURITY.md](SECURITY.md)**, and please do not open a public issue for it.

### What makes a report we can act on

Not length. These four lines, roughly:

1. What you were trying to do.
2. What you did — the exact steps, or the exact command.
3. What happened, including the error, in full.
4. What you expected instead.

Versions, browser and operating system if it is a front-end problem. And the
part everybody skips: **whether it happens every time**, because "sometimes" and
"always" are two completely different investigations.

---

## Response times, honestly

We are a small team. Issues and pull requests get a first response within **five
working days**; security reports within **two**. Our support team and the
helplines above are staffed properly — this repository is not, and we would
rather tell you that than have you wait on it.
