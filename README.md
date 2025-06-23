# dotfiles

## Setup Emacs

Install & Setup chemacs2
```sh
# Set up directories for emacs distros and configurations
mkdir -p $HOME/.config/emacs-config
mkdir -p $HOME/.config/emacs-distro

# Clone chemacs2
git clone https://github.com/plexus/chemacs2.git $HOME/.emacs.d

# Link dotfiles `.emacs-profiles.el` to users `$HOME` directory
ln -s $(git rev-parse --show-toplevel)/.emacs-profiles.el $HOME/.emacs-profiles.el
```

Setup spacemacs
```sh
# Clone spacemacs
git clone https://github.com/syl20bnr/spacemacs.git $HOME/.config/emacs-distro/spacemacs

# Link dotfiles `.spacemacs.d` to users `.config/emacs-config` directory
ln -s $(git rev-parse --show-toplevel)/.spacemacs.d $HOME/.config/emacs-config/.spacemacs.d
```
