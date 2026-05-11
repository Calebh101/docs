---
title: Account Deletion Emails
parent: Emails
nav_order: 3
---

# Account Deletion Request

This is sent to you when you try to delete your account at [account.calebh101.net](https://account.calebh101.net). You will be sent the following details:

- Email of account: The email of the account changing their email.
- Verification code: A code for the verification link. Note that this changes in between the first verification and the second.
- Session ID: The session ID of the user doing this. **Make sure you check this against what you see under "Current session ID" on the device doing this change.**
- IP address: The IP address of the user requesting this.
- User agent: The user agent of the device requesting this. See [the glossary](../glossary.md#user-agent) for more info.

### The Link

When you click the link, it doesn't immediately delete your account; it just leads you to a page with a big `Delete` button.

When you click Delete, you will be presented with a confirmation, then your account will be deleted. **This is not recoverable; all of your data is immediately deleted from the database.**

But here's the parts of the link, if you're curious:

```https://account.calebh101.net/?p=deleteAccount&code=hf629f&session=jf74jg92o82f```

- `account.calebh101.net/`: My website.
- `?p=deleteAccount`: Tells the website to go to the verify old email page. `p` means "page".
- `&code=code`: Autofills the verification code field.
- `&session=sessionid`: Autofills the session ID field.

You can go to [https://account.calebh101.net/?p=deleteAccount](https://account.calebh101.net/?p=deleteAccount) manually to fill out these fields; this extra long link just does this for you.

# Account Deleted

This is sent to you when your account was successfully deleted. You'll be sent the following details:

- IP address: The IP address of the user requesting this.
- User agent: The user agent of the device requesting this. See [the glossary](../glossary.md#user-agent) for more info.

This email is sent as a notice, so there's no action to do.