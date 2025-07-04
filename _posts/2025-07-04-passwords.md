---
layout: post
title: What is a "Strong" Password?
date: 2025-07-04
published: true
---

You hear all the time that you should be using "Strong Passwords", but what does that mean, exactly? Do I need a complex password, a long one, both? How do password strength meters work? In this article I hope to shed some light on these topics.

For this article, we will define a strong password as follows:

*A strong password is one that is difficult for an adversary to guess, whether by brute force, educated speculation, or specific intelligence.*

Lets break that down.

## Difficult for an adversary to guess
This simply means you and only you should control who has this password. There should not be a way for someone other than you to have the password without you giving it to them, or them stealing it from you. (Securing password storage is an important topic, but outside the scope of this article.)
The adversary or attacker is some other party who is attempting to use your password without your consent. These terms are preferable to "hacker" because they are more generic and less loaded.

## Brute force
In simple terms, this means the attacker guesses every possible permutation of a password until they find yours. With modern computing power, anything 8 characters or less is relatively trivial to break with this method (Presuming the attacker does not have a limited number of attempts.)

## Educated Speculation
In essence this part means that if the attacker is able to guess how you made the password, that should not give them enough of an advantage to be able to break the password. In other words, the security of the password should not depend on obscuring its method of creation.
Security through obscurity is only as secure as it is obscure, and will only remain obscure for a finite period. It is far more reliable to have a password that is mathematically secure even when the adversary knows exactly how you made it.

## Specific Intelligence
The essence of this criterion is, there should not be a piece of information an attacker targeting you could find out that would reveal the password to them, or make it significantly easier to guess. 
Do not use any personally identifiable info in your password, such as birthdays, pets names, or anything else of the sort in your passwords. Anyone could easily find this information on Facebook, Instagram, and other social media sites where you have revealed this, or from public records and various data broker sites where you don't even have control over what gets shared. As a sidenote, this is why security questions to recover accounts are generally considered to be highly insecure. If you are forced to use them, give gibberish answers and write those down in a safe place rather than using the truth. The answers to those questions can usually be found for free, without much effort, if someone decides to look.

Secondly, and more importantly, don't use duplicate passwords. If you do, no matter how strong the password, as soon as one account with the password is hacked, all of your accounts with that password are in the same boat. Once one password is leaked or stolen, attackers will try that email and password combination on any site they want. If you reused the password, they now have easy access to multiple of your online accounts, not just one.

## Calculating password strength
Complexity requirements for passwords are bad. They make the password less secure in some ways, because there are parameters that the adversary knows to refine their search, but more importantly, it is more difficult for the user, which means the user will likely do other bad things to circumvent it such as reusing the same password or storing it in an insecure location.


Really, you should not use anything at all for a password that is not randomly generated. Anything that is not, such as regular English phrases, things you come up with in your head, or the items that happen to be on your desk, have patterns and lead to weaker passwords. A randomly generated password has no such patterns. It does have patterns, but for well-known methods those patterns have been determined and added to the process of calculating their security. A known is far better than an unknown in this scenario.

Now how would I know what mathematically complicated is?

Well, it's complicated. ;P

log(2)N is the equation to calculate entropy or randomness (for our purposes here, it's actually a bit more complicated). This assumes brute force guessing. For an all-lowercase alphabet only password, 

`N=26^l`

where **l*** is the number of characters in the password.
So if we have a 10-character password, N will equal 

`26x26x26x26x26x26x26x26x26x26`

Entering that into our equation, 
`log base 2 of (1.4e14) EDIT`,
we get an entropy value of 47 bits.

This is not a secure password. As of 2023, 90 bits is considered pretty secure. To up the entropy of our password, we can add length (more from our alphabet or character set) or complexity (add more characters to our character set). [Add more examples of better passwords, with the maths. Maybe also add built-in calculator?] This is where the idea of a *passphrase* comes in. Instead of a string of characters, a passphrase is a string of words, such as *correct horse battery staple*. Diceware-style passphrases do both. Diceware uses a set of 7776 words to make a passphrase from. This is as if our alphabet is now 7776 words long. Much better than 26. And if someone assumed we were using the 26 letter alphabet character set (with spaces) then we have length too. We can also add a number or symbol to the start or end of one of our words for added complexity


did3o(*d0fds0*0073 vs *correct horse battery staple*
Explain How passphrase with wordlist is still secure and better than random
*refer to calculations*
*note that you can actually remember one of them*
*if you're entering in public, harder to shoulder surf because you don't need to show the password/can type it faster*

## What about my phone/bank/etc PIN?
In short, though these are cryptographically weak due to the limited alphabet and length, they are secure enough because there are other measures preventing many password attempts or securing the data through other factors.

## Conclusion
If you take nothing else away from this article, remember this: Use unique, randomly generated passwords for every account, and store them somewhere safe like a password manager. If you're choosing one to use, evaluate password managers based on their handling of sensitive data, transparency with regular third-party audits, cryptography, and competency in response to security incidents when they happen.

And lastly, I hope you learned something interesting!



*Links*

[useapassphrase.com](https://www.useapassphrase.com)

[xkcd 936 (comic illustrating passphrase advantages)](https://xkcd.com/936/)

[Don't pass on the new NIST password guidelines](https://auth0.com/blog/dont-pass-on-the-new-nist-password-guidelines/)

[Article from 2012 on password strength checkers](https://dropbox.tech/security/zxcvbn-realistic-password-strength-estimation)

[Diceware](https://theworld.com/~reinhold/diceware.html)

[EFF Dice-Generated Passphrase](https://www.eff.org/dice)

[Don't use LastPass: Analysis of their awful response to multiple breaches](https://palant.info/2022/12/26/whats-in-a-pr-statement-lastpass-breach-explained/) 

[Post by security researcher on LastPass](https://infosec.exchange/@epixoip/109585049354200263).

[Electronic Frontier Foundation on Password Managers](https://ssd.eff.org/module/animated-overview-using-password-managers-stay-safe-online)

[Interesting article on the downsides of password manager browser extensions](https://lock.cmpxchg8b.com/passmgrs.html)
