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

### Directories and Files

| Function                     | Key            | Plugin                                                                                                                                                                                                  |
|------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| List directory               | `<Alt+l>`      | Core fish functionality                                                                                                                                                                                 |
| Search in directory          | `<Ctrl+f>`     | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish)                                                                                                                                             |
| ... then open in editor      | ... `<Ctrl+e>` | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish)                                                                                                                                             |
| ... then open with xdg-open  | ... `<Ctrl+o>` | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish)                                                                                                                                             |
| ... then toggle preview      | ... `<Ctrl+t>` | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish)                                                                                                                                             |
| Change into directory        | `<Alt+c>`      | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish) + [custom function](https://github.com/mbollmann/linux-essentials/blob/master/dot-files/.config/fish/functions/__mmb_change_directory.fish) |
| Change into hidden directory | `<Alt+C>`      | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish) + [custom function](https://github.com/mbollmann/linux-essentials/blob/master/dot-files/.config/fish/functions/__mmb_change_directory.fish) |
| Open Dired                   | `<F5>`         | [mbollmann/emacs.fish](https://github.com/mbollmann/emacs.fish) + Emacs                                                                                                                                 |

### Commands and Processes

| Function                       | Key            | Plugin                                                      |
|--------------------------------|----------------|-------------------------------------------------------------|
| Search command history         | `<Ctrl+r>`     | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish) |
| Search saved snippets          | `<Ctrl+s>`     | [mbollmann/pet.fish](https://github.com/mbollmann/pet.fish) |
| Save new snippet               | `<Ctrl+Alt+n>` | [mbollmann/pet.fish](https://github.com/mbollmann/pet.fish) |
| Comment/uncomment current line | `<Alt+'>`      | Core fish functionality (defaults to `<Alt+#>`)             |
| Search processes               | `<Ctrl+Alt+p>` | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish) |
| Search environment variables   | `<Ctrl+v>`     | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish) |


### Git functionality

| Function                 | Key            | Plugin                                                                                              |
|--------------------------|----------------|-----------------------------------------------------------------------------------------------------|
| Open Magit status window | `<F4>`         | [mbollmann/emacs.fish](https://github.com/mbollmann/emacs.fish) + Emacs + [Magit](https://magit.vc) |
| Search git log           | `<Ctrl+Alt+l>` | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish)                                         |
| Search git status        | `<Ctrl+Alt+g>` | [PatrickF1/fzf.fish](https://github.com/PatrickF1/fzf.fish)                                         |
