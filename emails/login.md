---
title: Login Emails
parent: Emails
nav_order: 1
---

Did you receive a login email? Cool, that means my code worked.

If you're curious about the different types, and what each link means, you're in the right place! I created this so the links in my emails don't look like big sketchy things you don't want to click.

[Verify Your Email](#verify-your-email): Verifying your email when you create a new account.<br>
[Verify Your Login](#verify-your-login): Verifying your device when signing in.

## Verify Your Email

With this email, you'll receive a few things:

- A session ID. This is so only your device, and your email, can use the code we sent you. You normally don't need to worry about this, unless you're typing details in manually.
- A verification code. This is the actual code, and only your email will have it. This is also normally handled for you, like the session ID.
- The IP address trying to log you in.
- The user agent of the device trying to log you in. See [the glossary](../glossary.md#user-agent) for more info.
- A link.

### The Link

When you click the link, it doesn't immediately verify the email; it just leads you to a page with a big ol' `Verify` button. Clicking that verifies your email.

But here's the parts of the link, if you're curious:

```https://account.calebh101.net/?p=verifyEmail&email=me%40gmail.com&code=hf629f&session=jf74jg92o82f```

- `account.calebh101.net/`: My website.
- `?p=verifyEmail`: Tells the website to go to the verify email page. `p` means "page".
- `&email=your email`: Autofills the email field.
- `&code=code`: Autofills the verification code field.
- `&session=sessionid`: Autofills the session ID field.

You can go to [https://account.calebh101.net/?p=verifyEmail](https://account.calebh101.net/?p=verifyEmail) manually to fill out these fields; this extra long link just does this for you.
Hope this clears some stuff up!

## Verify Your Login

This email just contains a 6-character 2-factor-authentication (2FA) code. It also includes the IP address and [user agent](../glossary.md#user-agent) of the device trying to log in.
