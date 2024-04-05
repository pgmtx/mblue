+++
title = 'Which mobile pdf reader should you use?'
date = 2024-04-02T21:02:57+02:00
draft = false
+++

## Introduction

I was looking for a new pdf reader, so I dug on AlternativeTo.

I ditched Google Drive, so no pdf reader from Google. Xiaomi one has contrast issues (in terms of display). So let's see if open source apps are interesting in that domain.

## Sav Pdf Reader

Welcomes me with a "choose your file" screen, but once I select one, the app crashes. It didn't ask for permissions to access file storage, so I guess that is the cause.

## MuPdf

The first alternative pdf reader I used to replace Google and Xiaomi ones.

It has a word finder and you access other pages by scrolling left or right, which disturbed me at first use. For short files, no problem. But it becomes horrendous for files with multiple pages.

To resolve that, MuPDF can display the table of content, or you can use the slider. If you can't see it, you simply have to tap on the screen, then you use the slider to go to directly to the page you want. The only complain I have is the fact that the slider is set a little too low on the screen, so it might be annoying if you have a phone with big screen or if you just want to use the app with only one hand.

![An overview of MuPdf](/images/mobile-pdf-reader/mupdf.png)

You might wonder what the button with the chain icon does. Unfortunately, I don't know. Activating or deactivating it doesn't change anything.

The application works perfectly **if you're on light mode**. On dark mode some pages are white, other ones are black, and zooming in and out changes the color. There are no settings, so you can't help but deactivate your dark mode if you wanna use it in optimal conditions.

Also, MuPDF sometimes offers to open file formats it doesn't support (like maff). Very odd.

It supports epub format, but the reading is definitely not optimal. I recommend it only for pdf files.

## MJ Pdf Reader

Looks more modern, more recent. Allows you to read on full-screen, auto-scroll, lock the zoom or the horizontal scroll, and offers you to read files with a bright or dark theme.

Great! But it has the same problem as MuPDF : if your phone is on dark mode and MJ treats your files with the bright theme, you get an inconsistent rendering.

![What inconsistent rendering looks like](/images/mobile-pdf-reader/mjpdf.png)

To fix that, tap on the three points on the right, then "more" and "app settings" (looks strange to set the settings button apart, but the option is very appreciable). All the way down, activate "PDF pages follow system theme", and voila.

Dark theme works well tho, but looks more like a negative one. Not everyone will like it, and personally I'm not sure I'd use it all the time.

![Dark theme only](/images/mobile-pdf-reader/negative.png)

## Secure Pdf viewer

You can jump on any page with this one, but you have to scroll, instead of writing directly the page number. Clearly, this is not ideal if you have a document with a thousand pages.

![How to jump to page](/images/mobile-pdf-reader/jump.png)

Another thing that disturbs me : you navigate from left to right, but you can't swipe. So you have to tap on the arrows at the top of the screen. And it doesn't have settings.

One notable thing, each time you open a file, another instance of the app is created, even if it's the same file. A bit overwhelming.

![Multiple instances on my phone](/images/mobile-pdf-reader/instances.png)

Anyways, it's a decent viewer, and has no rendering issues if you use dark mode (but has no dark theme).

## Document Viewer

Obtainium showed me five versions available, but only 2821 and 2822 were installable, other ones had a pop-up about incompatibility.

First thing I noticed : the interface is AWFUL.

![Really, really awful](/images/mobile-pdf-reader/interface.png)

Seriously, I hesitated reviewing this app since it was discontinued. I don't mind the old UI for the settings (even though the categories should have been clearer and rearranged), but the first impression is important.

Some files are shown with an inverted theme for no reason.

![Why](/images/mobile-pdf-reader/inverted.png)

The only thing I like is that the files content you already opened are now shown on the feed.

![This is nice actually](/images/mobile-pdf-reader/content.png)

Additionally, it can open other file formats, such as epub, but in that case it would have been better to show file extensions.

Oh, and Document Viewer seems to have security holes, so I wouldn't recommend it.

## Orion Viewer

Old interface, and **no search capacity**. Only throws your folders and you have to manage on your own. At least it shows pdf files only.

![The interface](/images/mobile-pdf-reader/orion.png)

Ah and, when you open a file, you'll be greeted with this screen.

![A disturbing screen](/images/mobile-pdf-reader/screen.png)

There is a keyword search (the binoculars icon), and a go to option, but again it is a slider. It seems you can bookmark pages, that you can see then on the bookmarks option. This is a nice feature, however you can't see directly and explicitly a bookmark page (it is not highlighted).

One very interesting feature, you can crop the pages! Pretty cool, and the zoom gestures works flawlessly.

The files are also sorted by name, not by date, which seems counter to the previous readers, but allows to find your files easily. But again, a search bar would be even more time-savior. It seems obvious, but as it is old enough, it is not affected by dark mode in any way.

## Conclusion

I guess the common issue with themes is not linked to the applications, but with my phone (or maybe MIUI).

To read pdf files, I'd suggest Secure Pdf Viewer, despite the lack of gestural features. If you work late, or just can't stand white pages, use MJ Pdf Reader, which looks very promising. If you don't have a lot of pdf files or you organize them correctly, it is not a bad idea to try Orion Viewer.

> Why aren't you writing PDF with all caps ?

I don't shout at people.

> Please make a tier list.

Not now, but soon maybe.

[Back to top](#introduction)
