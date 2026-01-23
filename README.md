# Dotfiles

Personal configuration files managed with GNU Stow and Git submodules.

## Prerequisites

Install GNU Stow:

```bash
sudo apt install stow  # Debian/Ubuntu
brew install stow      # macOS
```

## Setup

1. Clone with submodules:

```bash
git clone --recurse-submodules https://github.com/ahmednmourad/dotfiles.git
```

Or if already cloned:

```bash
git submodule update --init --recursive
```

2. Stow packages:

```bash
stow <package1> <package2> ...
```

Example:

```bash
stow zsh oh-my-zsh
```

## Update Plugins

```bash
git submodule update --remote
```
