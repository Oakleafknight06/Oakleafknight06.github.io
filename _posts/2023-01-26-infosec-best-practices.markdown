# Information Security Best Practices Compilation

## Recommendations

- **Keep software up to date.**
Don’t use an unsupported version of macOS, Windows, (8.1 and earlier), or anything else (iOS, Android, Linux). Don’t use a version of Android which is no longer receiving monthly security patches.

If your device does not support a new version, try Linux on desktops or laptops, and LineageOS (if supported) on your Android phone. You don’t really have alternatives for iPhone, but one thing Apple does quite well is providing long software support, so it is likely you are due for an upgrade for other reasons too.

- **Use a (secure) password manager**

	- Online passsword managers

		[Bitwarden](https://bitwarden.com)

		A FOSS password manager. Can be self-hosted if desired

		[1Password](https://1password.com) 

		Not FOSS, but has regular audits and works closely with password cracking community

	- [KeePass](https://keepass.info) (FOSS, A file format, compatible with many clients)

		[KeePass XC](https://keepassxc.org/) Windows/macOS/Linux (free)

		[KeePass DX](https://www.keepassdx.com/) Android (free)

		[KeePassium iOS](https://keepassium.com/) (paid)


[Do](https://palant.info/2022/12/26/whats-in-a-pr-statement-lastpass-breach-explained/) [not](https://infosec.exchange/@epixoip/109585049354200263) use LastPass.

Evaluate password managers based on their handling of sensitive data, transparency with regular third-party audits, cryptography, and competency in response to security incidents when the happen. (These guidelines are also helpful when evaluating VPNs).

- **VPNs are not a security or privacy tool. They are for circumventing censorship.**

They can be useful tools, however. [Mullvad](https://mullvad.net/en/) is one of the best. [Mozilla VPN](https://www.mozilla.org/en-US/products/vpn/) uses their servers as well. [ProtonVPN](https://protonvpn.com) is also a good option, especially if you already use ProtonMail.

- **Use two-factor authentication (2fa)**

Time-based One Time Password (TOTP, the one with 6 numbers that rotate on a timer) is the most common standard. If something says it supports Google Authenticator or Authy this is what it supports. Aegis for Android, Ravio on iOS.
Only use sms for two factor when there is no other option, and even then use a VOIP number such as…

- **Google Voice**

Yes, they’ll use the data to advertise you, but you might trust them more than your cell provider and you can prevent someone else from getting your cell number by bribing an underpaid cell service employee.

- **Additional Notes Regarding SMS**

SMS is one of the least secure forms of online communication avaliable. Thus it shoudld not be trusted with anything sensitive. In many cases, not using two-factor authentication at all would be more secure. Refer to this [podcast episode](https://malicious.life/episode/episode-204/) for some more information on sim swap attacks.
     For communication purposes, it is fine to use but is unencrypted and any information sent through it should be treated as publicly available.

- **Use a privacy-respecting open source browser such as Firefox or Brave**

- **[Full disk encryption](https://ssd.eff.org/glossary/full-disk-encryption) on your computer(s)**
(Your phone will have this by default most likely)


- **Secure open-source text/voice messaging**
Such as [Signal](https://signal.org) or [Session](https://getsession.org)


- **Use Cloudflare’s 1.1.1.1 DNS on your routers and devices**


- **Use a secure email address from a provider for whom you are not the product (ie usually paid).**
ProtonMail and Tunatoa are good

- **Monitor your accounts to see when (not if) they get compromised.**

	- [HaveIBeenPwned](https://haveibeenpwned.com/)  

	- A Firefox account & [Firefox Monitor](https://monitor.firefox.com/) makes this easier.

- **If you don’t need it, don’t install it.  If you’re not using it, uninstall it.  If you didn’t ask for it, don’t click on it.**

- **Any recovery method is an attack vector**

An attacker need only break the weakest link in the chain. This is particularly relevant in the case of a password hint or security questions. There is no good reason to use a password hint (insert article). Security questions based on real facts about you are very insecure, because much of that information is freely avaliable or not hard to find. If you need to use security questions, treat them as another password feild.
     Secondly, if an account can be recovered via email or sms without knowing the password and/or having access to a 2fa device, the security of the account is only the security of the email or sms.
     And a final note, when setting up 2fa you will get recovery codes of some sort. Store these safely, as again they are a recovery method by which an attacker could gain access to your account. (They are also how you gain access if you forget your login details or lose your second factor device)


## Explainers and how-tos for the above
**2FA/MFA: What they are and how to use them**

[EFF article](https://ssd.eff.org/module/how-enable-two-factor-authentication)

[Tom Scott video](https://www.youtube.com/watch?v=hGRii5f_uSc)


## Miscellaneous useful resources

From ProtonMail.com

[For individuals](https://proton.me/support/new-account-owner-security-checklist?utm_campaign=ww-en-2c-generic-coms_email-monthly_newsletter&utm_source=proton_users&utm_medium=link&utm_content=2021_-_feb)

[For businesses](https://proton.me/business/security-guide?utm_campaign=ww-en-2c-generic-coms_email-monthly_newsletter&utm_source=proton_users&utm_medium=link&utm_content=2021_-_feb)

Why weak encryption or giving governments a backdoor to WhatApp (Or Signal or any other secure communication) is a *very* bad idea: 
   [Why The Government Shouldn't Break WhatsApp](https://www.youtube.com/watch?v=CINVwWHlzTY)