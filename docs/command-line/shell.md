---
title: Shell
parent: Working on the Command Line
layout: default
nav_order: 3
---

# The Shell

## fish

The default shell on most Linux systems is the [Bash
shell](https://en.wikipedia.org/wiki/Bash_(Unix_shell)), and you can't go wrong
with learning how to use it. However, I made the switch to
[**fish**](https://fishshell.com/) a couple of years ago and now I never want to
use anything else.

What's nice about the [fish shell](https://fishshell.com/) is that it offers autosuggestions, tab completions, syntax highlighting, and is easy to customize and write scripts for.
{: .callout .callout-primary }

Fish can suggest completions for executables, paths, options, and even full
command invocations from your history.  Press tab to easily accept these
completions.  Syntax highlighting will furthermore tell you if a command exists
& is executable, if a given file path is valid, or if you forgot the closing
quotes on a string, _all before you ever press "Enter"._

PLACEHOLDER

There's one potential downside, which is that fish is not POSIX-compatible,
meaning that if you're used to Bash syntax, you might have to relearn a few
things.  In practice, I've never found this to be a huge issue.  Some common
differences that you quickly to get used to are:

1. Slightly different keywords for loops and conditions:
   - `for ...; do_something; end` _(fish)_
   - `for ...; do do_something; done` _(bash)_
2. Command substitutions without a dollar sign:
   - `echo (command)` _(fish)_
   - `echo $(command)` _(bash)_
3. Declaring variables:
   - `set foo "bar"` _(fish)_
   - `foo="bar"` _(bash)_

The fish documentation has [a comprehensive overview of the differences to Bash
syntax](https://fishshell.com/docs/current/fish_for_bash_users.html), but also,
remember that even if you set fish as your default shell, Bash is still there
for you—you can still write & run Bash scripts if that's what you're more
comfortable with for a given task.  The syntactic differences are mostly
relevant for writing quick one-liners directly on the command line.

## fzf (Shell extension)

One bonus of fish is its easy extensibility.  [**fzf** ("fuzzy
finder")](https://github.com/junegunn/fzf) is a command-line tool for finding
things, but also works as an [awesome fish
extension](https://github.com/jethrokuan/fzf).

Want to `cd` into some deeply nested directory like
`~/Documents/Courses/Intro_to_programming_2021/assignments/week3/`?  That's a
lot of keys to press, even with the help of tab completions.  How about just
typing `<Alt-C> week3 <Enter>`?

What was that long one-liner you used a few months ago, of which you remember
nothing except that one of its arguments was a file named `plot.pdf`?  How about
just typing `<Ctrl-R> plot.pdf` and seeing what comes up?  Of course, you could
also `grep` through your history file, but with fzf's `<Ctrl-R>` you get fuzzy,
interactive search, and if you find the command you were looking for, pressing
`<Enter>` on it will paste it directly onto your command line.

_(Note that fzf also [comes with built-in support for Bash
users](https://github.com/junegunn/fzf#fuzzy-completion-for-bash-and-zsh), but I
haven't tried that.)_

## Starship (Prompt)

TODO