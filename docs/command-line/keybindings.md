---
title: Keybindings
parent: Command Line
layout: default
nav_order: 20
---

# Keybindings

This section is mostly personal, as it describes keybindings that I've partly
re-configured for myself in [my
dot-files](https://github.com/mbollmann/linux-essentials), but it might still
serve as an inspiration for what you can do.

- - -

### fzf (search extension)

These keybindings relate to
[fzf.fish](https://github.com/PatrickF1/fzf.fish#search-commands), but are
customized from the default ones in my
[`config.fish`](https://github.com/mbollmann/linux-essentials/blob/master/dot-files/.config/fish/config.fish). "Change
into directory" and "Change into hidden directory" require a [custom function
defined
here](https://github.com/mbollmann/linux-essentials/blob/master/dot-files/.config/fish/functions/_fzf_mmb_change_directory.fish).

| Function                     | Key            |
|------------------------------|----------------|
| Search in directory          | `<Ctrl+f>`     |
| ... then open in editor      | `<Ctrl+e>`     |
| ... then open with xdg-open  | `<Ctrl+o>`     |
| ... then toggle preview      | `<Ctrl+t>`     |
| Search command history       | `<Ctrl+r>`     |
| Change into directory        | `<Alt+c>`      |
| Change into hidden directory | `<Alt+C>`      |
| Search git log               | `<Ctrl+Alt+l>` |
| Search git status            | `<Ctrl+Alt+g>` |
| Search processes             | `<Ctrl+Alt+p>` |
| Search environment variables | `<Ctrl+v>`     |

