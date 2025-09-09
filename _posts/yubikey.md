---
layout: post
date: 2025-07-24
published: false
---

This is my sharing of personal documentation as I figure out what I can use my Yubikey 5 NFC for, which I received from a friend. I hope it can be a helpful compilation of information for you too.

[YSA-2024-03](https://www.yubico.com/support/security-advisories/ysa-2024-03/)
Affects keys firmware older than 5.7
If you're just experimenting though, you're probably fine. 

## YubiKey Features
- FIDO
- OATH TOTP/HOTP
- Certificates (PIV).. how do I use these?
- Slots ~ they're versatile. Only 2 though
    - Long press and short press
    - Yubico OTP
    - Challenge-response
    - Static password
    - OATH-HOTP
## YubiKey PINs
https://support.yubico.com/hc/en-us/articles/4402836718866-Understanding-YubiKey-PINs
only 8 tries for FIDO. Thus 4 or 6 digit numerical pin should be alright, if it's random.

## Yubico software (on linux)
https://support.yubico.com/hc/en-us/articles/360016649039-Installing-Yubico-Software-on-Linux

## (Y)user Guide
https://docs.yubico.com/software/yubikey/tools/authenticator/auth-guide/settings.html#settings-home-pin-complexity
https://docs.yubico.com/software/yubikey/tools/authenticator/auth-guide/piv-certificates.html
