---
title: Email-Related Emails
parent: Emails
nav_order: 2
---

# Email Change Request

This is sent to you when you try to change your email at [account.calebh101.net](https://account.calebh101.net). This is sent to both your old address and your new address. You will be sent the following details:

- **IF sent to your old address:** New email (changing to): What your email will become after this change.
- **IF sent to your new address:** Email of account: The email of the account changing their email.
- Verification code: A code for the verification link. Note that this changes in between the first verification and the second.
- Session ID: The session ID of the user doing this. **Make sure you check this against what you see under "Current session ID" on the device doing this change.**
- IP address: The IP address of the user requesting this.
- User agent: The user agent of the device requesting this. See [the glossary](../glossary.md#user-agent) for more info.
- Location: The approximate location of the device requesting this. This is not accurate and is not always correct.

### The Link

When you click the link, it doesn't immediately verify the request; it just leads you to a page with a big ol' `Verify` button. Clicking that will move to the next step in the process, which is emailing your *new* email.

But here's the parts of the link, if you're curious:

```https://account.calebh101.net/?p=changeEmail1&code=hf629f&session=jf74jg92o82f```

- `account.calebh101.net/`: My website.
- `?p=changeEmail1`: Tells the website to go to the verify old email page. `p` means "page".
- `&code=code`: Autofills the verification code field.
- `&session=sessionid`: Autofills the session ID field.

You can go to [https://account.calebh101.net/?p=changeEmail1](https://account.calebh101.net/?p=changeEmail1) manually to fill out these fields; this extra long link just does this for you.

# Email Changed

This is sent to you when your email was successfully changed. This is sent to both your old email and your new email, both at the same time. You'll be sent the following details:

- Old email
- New email
- IP address: The IP address of the user requesting this.
- User agent: The user agent of the device requesting this. See [the glossary](../glossary.md#user-agent) for more info.
- Location: The approximate location of the device requesting this. This is not accurate and is not always correct.

This email is sent as a notice, so there's no action to do.