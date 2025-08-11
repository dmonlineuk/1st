# First Install

Some quick-access scripts to get started with a new install

## FIRST

If it's not already part of the initial install (I mean, reading this locally without git??), then install some required packages:

```bash
sudo pacman -S \
    git \       # Obvious?
    firefox \   # Browser?
    bat \       # View text files the best way possible
    stow \      # Improves dotfiles management
    tmux \      # Improves tty/pts use
    vifm \      # Required for aurutils
    less        # Required for `git diff`
```

## AUR

Two useful scripts in the subfolder `aurutils/`
- read both scripts before executing
- run the first script
- change a file: `/etc/pacman.conf`
- run the second script

Purpose is to:

1. Install the aurutils package from the AUR
1. Apply changes to the pacman conf to use the AUR
1. Ensure the link between AUR and pacman with the local repo
1. Reinstall aurutils with aurutils (as a test)

