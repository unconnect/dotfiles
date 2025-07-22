# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a personal dotfiles repository designed to manage and sync configuration files across multiple systems using GNU Stow for symlink management. The repository contains configuration files for various applications organized in separate directories.

## Architecture

- **Structure**: Each application has its own directory (neofetch/, rofi/, tilix/) containing config files in their expected `.config/` subdirectory structure
- **Deployment**: Uses GNU Stow to create symlinks from the dotfiles directory to the actual config locations in the home folder
- **Organization**: Follows XDG Base Directory specification with `.config/` subdirectories

## Key Components

### Configuration Directories
- `neofetch/`: System information display tool configuration
- `rofi/`: Application launcher and window switcher with custom themes and applets
- `tilix/`: Terminal emulator configuration

### Rofi Configuration
- Main config: `rofi/.config/rofi/config.rasi`
- Custom applets in `rofi/.config/rofi/applets/bin/` for system functions (power menu, volume, brightness, etc.)
- Multiple theme variants in `applets/type-*/` directories

## Essential Commands

### Deployment
```bash
# Deploy a specific configuration (run from dotfiles directory)
stow foldername -R

# Example: Deploy rofi configuration
stow rofi -R

# Remove/restow configuration
stow foldername -R
```

### Dependencies
- Requires `gnu-stow` package to be installed