# Fabio's .dotfiles

## Overview
I manage my `.dotfiles` using gnu stow.

For example for my nvim configuration I just did the following:


```sh
mkdir -p ~/.dotfiles/nvim/.config
mv ~/.config/nvim ~/.dotfiles/nvim/.config
```

At this point my nvim configuration is now tracked in this git repository. All changes I make to my nvim configuration can now
be saved so that I can use them on any machine.

Now on any machine I can simply do inside of the `.dotfiles` directory:

```sh
stow nvim
```

The key here is that once you are inside `~/.dotfiles/nvim`, it's as if you are in `~/`
