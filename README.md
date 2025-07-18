# My personal dotfiles

This repo is dedicated to manage and sync my config files between multiple systems.

This folder is suited to be used with [gnu-stow](https://www.gnu.org/software/stow/) for easy symlinking the between dotfiles-folder and the actual locations in my home folder.

Run
```bash
$ stow foldername -R
```
in the dotfiles folder. gnu-stow will symlink the configs to it's defined destination.
The destination is based on the folder structure inside the respective folder.

## TODO
- [ ] .zshrc
  - [ ] split in multiple files by usage: aliases, etc. pp.
- [ ] vim / neovim
- [ ] calculator for rofi?
- [ ] Add doc how to use this with gnu stow
- [ ] git config
- [ ] profile
- [ ] fzf
- [ ] bashrc
- [ ] timeshift
- [ ] backup
