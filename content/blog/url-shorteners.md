+++
title = 'Rating url shorteners'
date = 2024-07-25T17:47:07+02:00
draft = false
tags = [
  "open-source",
]
+++

## Introduction

Recently I wanted to invite someone on SimpleX Chat, but the invite links are
too long, which might look scary. That's why I'm looking for an (open source,
obviously) url shortener, so that links seem OK and concise.

I don't care about tracking the stats about the link (how many times it has
been clicked, what were the interactions, etc.), I simply want a software,
preferably online, to shorten urls I give to it.

## The holy table

| Name       | Checks links                                               | Has captcha                | Cloudflared | Note                                                       | Would I use it ? |
|------------|------------------------------------------------------------|----------------------------|-------------|------------------------------------------------------------|------------------|
| [Lstu]     | Yes, refuses to shorten links never opened before          | No                         | No          |                                                            | No               |
| [rs-short] | Yes, refuses if it was already flagged by the server admin | Yes, writing shown symbols | No          |                                                            | Probably         |
| [Ouvaton]  | No                                                         | Yes, resolving a sum       | No          |                                                            | Probably         |
| [v.gd]     | Yes, refuses if it is blacklisted                          | No                         | No          | Displays a page showing full link before redirecting to it | Probably         |
| [is.gd]    | Yes, refuses if it is blacklisted                          | No                         | Yes         |                                                            | No               |

[Lstu]: https://lstu.fr/
[rs-short]: https://s.42l.fr/
[ouvaton]: https://ouvaton.link/
[v.gd]: https://v.gd/
[is.gd]: https://is.gd/
