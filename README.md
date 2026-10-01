# Linux Workstation Setup & Dotfiles

Automated setup scripts, package lists, and configuration files (dotfiles) for deploying a clean, reproducible Linux workstation environment.

## Overview

This repository contains terminal configurations, shell aliases, application settings, and deployment scripts to quickly bootstrap a fresh Linux installation. It is designed to streamline system setup, enforce consistent environment settings, and minimize manual configuration.

## Repository Structure

```
.
├── bootstrap.sh              # Main installation and symlink script
├── config/
│   ├── .bashrc               # Main Bash shell configuration
│   ├── .bashrc_aliases       # Command shortcuts and custom aliases
│   ├── .gitconfig            # Git user config and global settings
│   └── .tmux.conf            # Terminal multiplexer settings
├── scripts/
│   ├── install_packages.sh   # System dependencies and APT/Flatpak installer
│   └── setup_desktop.sh      # UI layout, fonts, and theme customization
└── docs/
    └── post_install.md       # Post-installation checklist and manual steps
```

## Quick Start & Installation

### Clone the Repository

Clone the repository to your home directory:

```bash
git clone https://github.com/Duncan1738/Linux-Workstation-Setup-Dotfiles.git ~/dotfiles
cd ~/dotfiles
```

### Run Bootstrapper

Grant execution permissions and execute the bootstrap script to create configuration symlinks and install base dependencies:

```bash
chmod +x bootstrap.sh scripts/*.sh
./bootstrap.sh
```

## Included Configurations

### Shell & Environment
- Custom prompt configuration with Git status integration
- Essential safety aliases (`rm -i`, `cp -i`, `mv -i`)
- Navigation shortcuts and directory color settings

### Developer Tooling
- Global Git settings pre-configured for development
- Multiplexer layout for `tmux` with custom pane management
- Quick-install package lists for common development tools (`curl`, `git`, `htop`, `ripgrep`, `build-essential`)

## Author & License

Maintained by **Duncan1738**.

This project is open-source under the [MIT License](LICENSE).
