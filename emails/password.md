---
title: Password-Related Emails
parent: Emails
nav_order: 3
---

# Forgot Password

This is sent when you click Forgot Password. You'll be sent the following details:

- Verification code: The verification code for this password reset. Don't share this with anybody.
- IP address: The IP address of the user requesting this.
- User agent: The user agent of the device requesting this. See [the glossary](../glossary.md#user-agent) for more info.
- Location: The approximate location of the device requesting this. This is not accurate and is not always correct.

### The Link

When you click the link, it will lead you to a page to enter a new password.

But here's the parts of the link, if you're curious:

```https://account.calebh101.net/?p=forgotPassword&email=me%40gmail.com&code=hf629f```

- `account.calebh101.net/`: My website.
- `?p=forgotPassword`: Tells the website to go to the password reset page. `p` means "page".
- `&email=your email`: Autofills the email field.
- `&code=code`: Autofills the verification code field.

You can go to [https://account.calebh101.net/?p=forgotPassword](https://account.calebh101.net/?p=forgotPassword) manually to fill out these fields; this extra long link just does this for you.

# Password Changed

This is sent to you when your password was successfully changed. This is sent to both your old email and your new email, both at the same time. You'll be sent the following details:

- IP address: The IP address of the user requesting this.
- User agent: The user agent of the device requesting this. See [the glossary](../glossary.md#user-agent) for more info.

You'll also see one of two descriptions:
- "This was because of a password reset." Someone clicked Forgot Password to start the password reset.
- "Your password was changed while logged in." Someone clicked Change Password in the [account manager](https://account.calebh101.net) to reset your password.
- Location: The approximate location of the device requesting this. This is not accurate and is not always correct.

This email is sent as a notice, so there's no action to do.