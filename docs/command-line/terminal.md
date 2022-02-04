---
title: Terminal
parent: Working on the Command Line
layout: default
nav_order: 2
---

# The Terminal
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

- - -

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

- - -

## Emoji support

Does your terminal correctly render Unicode emoji?

```bash
echo "Emoji time!" 👍 🍎 🐜 🐻 🥖 🚌
```

In principle, if you're working in a graphical desktop environment, there's no
reason why it shouldn't, but you might have to tweak your system's font
configuration. Make sure you have [Noto Emoji
fonts](https://github.com/googlefonts/noto-emoji) installed (of course you can
also choose any other emoji font, like [JoyPixels](https://www.joypixels.com/)),
then create a file named `~/.config/fontconfig/conf.d/99-color-emoji.conf` with
the following contents:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE fontconfig SYSTEM "fonts.dtd">
<fontconfig>
  <alias>
    <family>monospace</family>
    <prefer>
      <family>Noto Color Emoji</family>
    </prefer>
  </alias>
</fontconfig>
```

Then, run `fc-cache -f` to rebuild your font cache. Finally, restart your
terminal application.

If that didn't do the trick, you could refer to [Victor Kropp's
blogpost](https://victor.kropp.name/blog/emoji-on-linux/) or [this GitHub
gist](https://gist.github.com/IgnoredAmbience/7c99b6cf9a8b73c9312a71d1209d9bbb)
for slight variations on the same idea.

- - -

## tmux / byobu

Especially when working on remote machines (e.g. via SSH), you want a way to
preserve your shell sessions and keep programs running after you log out. A good
way to achieve that is to [use a terminal multiplexer like
**tmux**](https://www.howtogeek.com/671422/how-to-use-tmux-on-linux-and-why-its-better-than-screen/). More
recently, I've discovered [**byobu**](https://www.byobu.org/), which builds on
tmux to provide an ever nicer user experience.

I need to use these tools more before I can give any practical tips here,
though.
