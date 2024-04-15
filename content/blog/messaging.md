+++
title = 'How to choose a messaging platform?'
date = 2024-04-07T16:19:29+02:00
draft = false
tags = [
  "messaging",
  "software",
  "open-source",
]
+++

## Introduction

Finding an messaging application to communicate with your family, friends and other acquaintances might be difficult.
It depends on your needs, whether you mind stepping out of your comfort zone, your threat modeling, etc.

Personally, my criterias are the following one:
1. Ideally, open source, because it allows more transparency and quick fixes.
1. Speed is essentiel: one second to send a message is okay, but not five or above (in the best conditions of course).

## SMS

Simple enough, but you need a flat fee. For some reasons, I can't send MMS when on Wi-Fi only. You can't create groups, and if you communicate with
someone abroad, you may have to pay fees. Clearly not ideal, so I add a third criteria:

3. The application should allow you to communicate with anyone from any country without constraints.

## WhatsApp

Probably the most popular app that respects the third criteria.

Requires your phone number. Has encryption, but the keys are held by Meta Inc., and your messages still transits to their servers. Moreover,
WhatsApp collects a lot of information.

One notable detail, which won't affect everyone : on Android, WhatsApp requires Google Services for notifications. As I disabled it, I sometimes don't
get push notifications, even when allowing the app to run in background. So most of the time I have to open it to read new messages that haven't appeared.

All of these flaws apply to **Messenger** as well.

## Discord

Discord [has](https://stallman.org/discord.html) [too](https://spyware.neocities.org/articles/discord) [many](https://usemumble.neocities.org/)
[problems](https://cadence.moe/blog/2020-06-06-why-you-shouldnt-trust-discord). In short, it collects much more data than necessary, can ban your account
for no reason, and adds questionable features that slow down your device.

And recently, Discord contradict itself by [planning to add sponsored ads](https://alternativeto.net/news/2024/4/discord-plans-to-introduce-sponsored-ads-for-revenue-contradicting-previous-stance/)
[[archive.is]](https://archive.is/dVmGN).

If you still need to use Discord, prefer using a client that blocks trackers, like [ArmCord](https://armcord.app/) (desktop) and [Aliucord](https://aliucord.com/) (Android).
These clients allow you to install mods as well, and, in theory, don't respect Discord's ToS. In practice, I got no problem with them and haven't been banned.

The issues with data collection leads me to another requirement:

4. The application should respect my privacy. If I'm not easy when someone listens to my private conversation with a friend in real life, then I don't
see why I would be by message. Therefore encryption is valued.

## Signal

The most popular privacy-oriented alternative to WhatsApp. Used it for a year to chat with my friends. Honestly, it works well. The similarities
with WhatsApp allow to reduce the learning curve.

Couldn't use it recently because I deleted the Google Services, and Signal needs them to work, otherwise you can't sign up.

## Session

A fork of Signal. The main difference is that you don't have to enter a phone number or username. Instead, a **unique id** is generated for you, which allows more anonymity.

I was ready to use it, but the biggest issue I met was the slowness of message sending and reception. Even with fiber and nearby devices,
messages took around ten seconds to be sent.

## SimpleX Chat

Let's go further : no phone number, no unique id made of random numbers. It only uses temporary ids that are different each time you connect.
The [website](https://simplex.chat/) gives clear and transparent information.

Unlike Session, the messages are sent and received instantly. However, I don't get any notification sound on my phone when I receive a message. I don't if it is a bug or a way to protect privacy, but it will be annoying for most people.
If you don't have any push notifications, meaning you have to open the app to get them, disable the battery saver for this app.

I haven't tried calls yet, so I can't tell about their quality.

I use it not only to speak with friends, but also to sync texts and files between my phone and my PCs, which is more ideal than using webapps such as
Pushbullet, Google Drive, etc.

In my opinion, the only considerable downside is the fact that you can't use the same profile on multiple devices, since there is no account system. 
Either you connect your phone profile to your pc, which is temporary, or you create a new profile on your pc, which works very well. Speaking of profiles,
creating one is very quick. So if you invite someone they won't have to setup a whole account with a phone number or anything. Another drawback I found: for some reason you can't download json files that you send or receive.

## Conclusion

Finding a messaging platform (or application in general) might be hard, so you have to dig a bit according to your needs.
I'd suggest SimpleX Chat, as it is only a question of time before fixing all these tiny flaws I tackled.

I haven't talked about similar services such as [Jami](https://jami.net/) or [Briar](https://briarproject.org/), 
since I never used them.
