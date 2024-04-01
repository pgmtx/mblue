+++
title = "Open source apps I'm using"
date = 2024-03-31T12:39:02+02:00
draft = false
+++

## Introduction

I will present open source apps that I use on my mobile phone.
My first motivation was that I accidentally removed Google Play store and service using adb.
So I had to find alternatives. I was looking for open source and straightforward applications, so that they are lightweight.

## App stores

First, I was using [F-Droid](https://f-droid.org/), but loading updates was slow, and for some apps you had to add external links, which behave 
like plugins.

By digging on AlternativeTo, I found [NeoStore](https://github.com/NeoApplications/Neo-Store), which is an F-Droid client with a modern UI and 
more features. I heard about [IzzyDroid](https://apt.izzysoft.de/fdroid/), but I haven't used it yet.

Next, I found [Obtainium](https://github.com/ImranR98/Obtainium), which allows you to install apps from their repository (Github, Gitlab, F-Droid).
Since in general, Github releases are more frequent than F-Droid, your apps will be more up-to-date. However, Obtainium is still in beta, so you might 
find some bugs.

Finally, if you'd like to install other applications, two words : Aurora Store. It's FOSS and you don't have to connect to your Google account to install applications.
And the timing is perfect, you can install it using Obtainium.

### For Xiaomi users

If you have a Xiaomi smartphone and you want to use NeoStore and/or Obtainium, you have to **disable MIUI optimizations**.

Here are the steps :

1. Go to `Settings > About phone`, and press the button "MIUI version" multiple times, until you get the message "You are now a developer".
1. No go to `Settings > Additionnal settings > Developer options`.
1. Scroll down, there should be an option "Disable MIUI optimizations". If not, in the Auto-fill section, tap multiple times on "Reset tp default 
values". Then you should find the desired option.
1. You will get a warning, tick the box, wait 10 seconds and press OK.

## Apps I'm using

All of them can be installed using Obtainium.

### ![](/images/open-source-apps/adaway.png) AdAway ![](/images/open-source-apps/adaway.png)

[AdAway](https://github.com/AdAway/AdAway) is a lightweight ad blocker. If your phone is non-rooted, it will use a VPN, else it will rewrite hosts file, which will be more optimized.
The downside is that, as it uses a VPN, you can't use other apps which work the same way, such as [NetGuard](https://github.com/M66B/NetGuard) or
[RiseupVPN](https://riseup.net/en/vpn/android) (probably the only free VPN that is legit).

Similar apps : [Blokada](https://github.com/blokadaorg/blokada), it lets you choose what kind of ads and trackers you want to block, but slows down 
much more your Internet connection.

### ![](/images/open-source-apps/amaze.png) Amaze File Manager ![](/images/open-source-apps/amaze.png)

[Amaze File Manager](https://github.com/TeamAmaze/AmazeFileManager) is a well-designed and highly customizable file manager.

### Ente Auth

Cross-platform.

Similar App : [Aegis Authenticator](https://github.com/beemdevelopment/Aegis) (Android only).

### ![](/images/open-source-apps/aves.png) Aves ![](/images/open-source-apps/aves.png)

[Aves](https://github.com/deckerst/aves) is an image and video gallery.

Before this, I was using Simple Gallery, and was pretty satisfied with it. However, Simple Mobile Tools got bought by a company, which then added
ads.

### Birday

Instead of taking notes of your relatives' birthdays, you can write them on [Birday](https://github.com/m-i-n-a-r/birday). It will gives you more 
information (age, astrological sign) and notify you when it's someone's birthday. You can also set reminders that notify you a few days before.

### ![](/images/open-source-apps/bitwarden.png) Bitwarden ![](/images/open-source-apps/bitwarden.png)

Freemium password manager.

### Clima

Get your meteo without having to indicate your geolocation. Has a black theme for AMOLED screens.

### ![](/images/open-source-apps/cromite.png) Cromite ![](/images/open-source-apps/cromite.png)

Bromite's last release is from 19 december 2022. So a fork has been created, [Cromite](https://github.com/uazo/cromite).

### FairEmail

Best email client.

### Feeder

Cool RSS feed reader.

### ![](/images/open-source-apps/floccus.png) Floccus ![](/images/open-source-apps/floccus.png)

A bookmark manager. To sync bookmarks, you need a nextcloud provider. Mine is [disroot](https://disroot.org/fr/services/nextcloud).
There is also an extension, which updates directly your browser bookmarks.

### Fossify Messages

Simple, private messages.

### ![](/images/open-source-apps/heliboard.png) HeliBoard ![](/images/open-source-apps/heliboard.png)

[HeliBoard](https://github.com/Helium314/HeliBoard) is a fork of OpenBoard.

### HuggingAssist

A HuggingChat client.

### MuPDF viewer

A simple, effective PDF reader. However pages become dark then light each time you change pages or zoom in/out.
If you know a better PDF viewer, feel free to send me a mail. I'll add here.

### Olauncher Clutter Free

A minimalist launcher, which removes ads, links from Olauncher and does not require Internet connection.

### OpenContacts

### OSS Docs Scanner

You take a photo, the app automatically detects document's border, and you can convert to pdf. Note that the app is updated VERY regularly.

### Quillpad

Take notes using Markdown.

### SimpleX Chat

Explain about Signal, Session, AlternativeTo etc.

### Misc.

Koler, Calculator, Camera.

[Back to top](#introduction)
