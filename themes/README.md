# Theme switcher for i3/Polybar

## Running playbook

```shell
[user@host themes] ansible-playbook -v set-theme.yml -e theme=example-theme
```

## Symlinks

Switching themes relies on the following symlinks being set

~/.config/i3/config -> ~/documents/dotfiles/themes/default/i3.config
~/.config/polybar/config -> ~/documents/dotfiles/themes/default/polybar.config
~/.Xresources.d -> ~/documents/dotfiles/themes/default
~/.Xresources -> ~/documents/dotfiles/.Xresources

You can then toggle between themes by changing the following symlink

~/documents/dotfiles/themes/default -> ~/documents/dotfiles/themes/{ theme }
