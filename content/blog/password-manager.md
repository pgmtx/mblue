+++
title = 'Use a password manager'
date = 2024-04-15T14:34:14+02:00
draft = false
tags = [
  "open-source",
  "social",
]
+++

## Introduction

Here I will list ways to store passwords, their flaws, and which one has more advantages.

## The paper way

Probably the first idea you get in mind, since it is accessible and easy to set up.
You write your passwords using a notebook. Do I need to explain why it is so
unsecure ? Fine, I'll do it :
- Anyone at your home could access it, so you have to hide it correctly.
- If someone finds it, they can read your passwords clearly.
- If you lose it, you lose all your passwords.
- If you share the notebook with another person, chances are you won't
remember where you left it *at least once*, and it will happen.
- If you're not at home (or another place you left the notebook) and need a
password you can't remember, it will be difficult to retrieve it. A call to a
relative might work, but clearly this is not ideal, and it causes an unnecessary stress.

If you live alone, then you have the advantage to trust only yourself to remember the location.

## The paper way, but unclear

Same as above, but you write your passwords in a different manner:

1. Find your way to create your password. For example, you replace every r occurrence by %, or every a by @.
1. Keep it in mind, then write the passwords without any symbol.

Example : for `M1st3%B3@st`, you would write `MisterBeast`.

The rules you're using in (1) to create your passwords from a basic expression is called **encryption**.

## Using your web browser

Please don't do this. These passwords are saved **in clear text**, so again
anyone using your PC can access it, including hackers.

## The password manager

One requirement : you have to remember one and only one password, called the
**master password**, and it has to be a minimum safe. Don't forget it,
otherwise you won't be able to recover your passwords.

### Advantages

With a password manager, you can fill automatically web pages asking for a
login and a password, and you can generate (and update) secure passwords easily,
according to you own criterias (length, minimum number of letters, digits, symbols, ...).

Last but not least, if you're using a cloud-based password manager, you have
synchronization, so you can instantly see changes between your PC and your
mobile phone.

### Downsides

A notable downside I found is when you want to fill in a password on a device
you don't use regularly : a computer at school, your friend's phone...

Here you have three solutions :

1. If you use a cloud-based password manager, connect to the website, so that you can
copy-paste the wanted password.
1. Otherwise, save your database file and the password manager executable on a
USB key, so that you don't even need to connect to a browser to get your
password. As I've been using a local password manager for a very short time, I
haven't applied the second solution yet.
1. If for some reasons you can't use the prior solutions, you can still look for
a password on your mobile password manager and type it character by character.
Clearly, this is the last resort solution, and I hate doing that. I leave it
here for sake of completeness.

## Choosing a password manager

There isn't a password manager that outperforms the others. It ultimately
depends on your needs. Paid solutions exist, but they add features in addition
of the password manager. For instance, Dashlane also includes a virtual wallet
as well as a VPN.

If you don't mind saving your data on cloud, a decent solution would be
[Bitwarden]. Even if it is freemium, you can use it without needing to pay, as
paid features here are not strictly necessary. You can also self-host it.

If you're more of a local person, you can use [KeePassXC] (desktop only). For
mobile phones, you can use [KeePassDX] / [KeePass2Android] or, for iOS, [Strongbox] / [KeePassium].

### Side note

If you're using the browser Librewolf, you won't be able to use KeePassXC
extension directly.

Here are the steps to fix that:

1. You have to create a special directory, by typing `mkdir ~/.librewolf/native-messaging-hosts`
on the terminal (note that I'm using Linux, so the path will vary for Windows).
1. Open KeePassXC desktop, then go to settings (the gear icon), browser
integration, and go to the *advanced* section.
1. Check "Use a custom browser configuration location:"
1. For *Browser Type*, select *Firefox*, and for *Config Location*, select the directory
`~/.librewolf/native-messaging-hosts`.

[Bitwarden]: https://bitwarden.com/
[KeePassXC]: https://keepassxc.org/
[KeePassDX]: https://play.google.com/store/apps/details?id=com.kunzisoft.keepass.free
[KeePass2Android]: https://play.google.com/store/apps/details?id=keepass2android.keepass2android
[Strongbox]: https://itunes.apple.com/us/app/strongbox-password-safe/id897283731
[KeePassium]: https://apps.apple.com/us/app/keepassium-keepass-passwords/id1435127111
