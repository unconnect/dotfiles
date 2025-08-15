# My personal dotfiles

This repo is dedicated to manage and sync my config files between multiple systems.

This folder is suited to be used with [gnu-stow](https://www.gnu.org/software/stow/) for easy symlinking the between dotfiles-folder and the actual locations in my home folder.

## Install dependencies

- git (Versioning all the files)
- gnu stow (Handles symlinking of the config files from dotfiles folder to there actual destinations.)

## Getting started

Clone dotfiles repo into homedir

```shell
cd ~/
git clone git@github.com:unconnect/dotfiles.git
```

Run stow in dotfiles dir. With package name for single package symlinking.

```shell
stow packagename
```

Restow, delete old symlink and link again.

```shell
stow packagename -R
```

Link all packages from stow dir (defaults to directory you are in eg. ~/dotfiles)

```shell
stow .
```


in the dotfiles folder. gnu-stow will symlink the configs to it's defined destination.
The destination is based on the folder structure inside the respective folder.

## TODO

- [x] Add doc how to use this with gnu stow
- [ ] .zshrc
  - [ ] split in multiple files by usage: aliases, etc. pp.
- [ ] vim / neovim
- [ ] calculator for rofi?
- [ ] zoxid
- [ ] eza
- [ ] git config
- [ ] profile
- [ ] fzf
- [ ] bashrc
- [ ] timeshift
- [ ] backup
