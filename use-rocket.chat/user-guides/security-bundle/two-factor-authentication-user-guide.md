---
description: Secure your account with two factor authentication.
---

# Two Factor Authentication User Guide

With the ability to extensively use Rocket.Chat on multiple platforms, and there is the risk of exposing your account details.

Rocket.Chat two-factor authentication (2FA) provides an additional layer of protection for workspace users by requiring them to provide two forms of authentication before accessing their accounts.

With 2FA enabled, a Rocket.Chat user is required to enter not only their username and password but also a one-time code generated by an authentication app, such as Google Authenticator, when logging into their account. This code is unique to each login attempt and provides an extra layer of security, as it cannot be reused or guessed.

{% hint style="info" %}
By default, 2FA is enabled with the email you used for signing up on the server.
{% endhint %}

To be able to use 2FA, the Rocket.Chat workspace administrator must turn on the Two Factor Authentication feature.

{% content-ref url="../../workspace-administration/settings/account-settings/" %}
[account-settings](../../workspace-administration/settings/account-settings/)
{% endcontent-ref %}

## Enabling Two Factor Authentication

{% hint style="info" %}
Before beginning the setup, download and have available any Authenticator app of your choice. Some popular Authenticators include [Google Authenticator](https://googleauthenticator.net/),[ Authy, ](https://authy.com/)and[ Duo](https://duo.com/).
{% endhint %}

To enable 2FA on your account,

* Click on your **User Profile**
* Navigate down to **My Account**
* Click **Security** to open up the security section
* Hit **Enable two-factor authentication via TOTP**
* Scan the QR Code provided with your Authenticator app or setup using the Authentication keys manually
* Copy the code displayed by the newly added Authentication means (`Rocket.Chat: <username>`) and fill in the field prompting to enter the code, then **Verify**
* A list of backup codes is provided. Save them securely in case you lose access to your Authenticator app
* After that, the 2FA setup is completed

{% hint style="info" %}
* TOTP is a Time-based One-Time Password. It is a very common form of 2FA.
* TOTP works by generating a unique numeric password with a standardized [algorithm](https://tools.ietf.org/html/rfc6238). The time-based passwords are made available and provide user-friendly, increased account security when used as a second factor.
{% endhint %}