---
title: Terminal
parent: Working on the Command Line
layout: default
nav_order: 2
---

# The Terminal

## Yakuake

A terminal emulator is the program that provides access to the command line, and
I've stuck with [**Yakuake**](https://apps.kde.org/yakuake/), a KDE-based drop-down
terminal, for many many years now.  I like the drop-down style of quickly
rolling the terminal down and up again, but the most important feature for me is
this:

I've made the `<F1>` key into a global shortcut for opening & closing my terminal.
{: .callout .callout-primary}

You can use other keys for that purpose, but I've never found that `<F1>`
conflicted with any function that I cared about in another program—typically it
is reserved for showing "help" screens.  You can also set this up with any other
terminal emulator, though Yakuake offers this functionality right out of the box.
The important thing here is that **I can open and close my terminal with the
press of a single key, no matter what I'm currently doing on my system.**  I've
found that super convenient.

## tmux / byobu

Especially when working on remote machines (e.g. via SSH), you want a way to
preserve your shell sessions and keep programs running after you log out. A good
way to achieve that is to [use a terminal multiplexer like
**tmux**](https://www.howtogeek.com/671422/how-to-use-tmux-on-linux-and-why-its-better-than-screen/). More
recently, I've discovered [**byobu**](https://www.byobu.org/), which builds on
tmux to provide an ever nicer user experience.

I need to use these tools more before I can give any practical tips here,
though.

## Emoji support

TODO
