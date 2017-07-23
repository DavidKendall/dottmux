# dottmux
A simple tmux configuration that uses
a [onedark theme](https://github.com/bk2dcradle/dotfiles/blob/master/tmux/themes/tmux.onedark.sh)

# Basic Installation

``` shell-session
$ cd ~
$ git clone https://github.com/DavidKendall/dottmux.git ~/.tmux
$ ln -s ~/.tmux/tmux.conf ~/.tmux.conf
```
You'll also need to configure your `.Xresources` file,
based on `~/.tmux/Xresources`.  (If you don't already have a `.Xresources`
file, you can just copy `Xresources` to `~\.Xresources`). See [this
note](http://www.futurile.net/2016/06/14/xterm-setup-and-truetype-font-configuration/)
for guidance on configuring `xterm`.

# Powerline

This configuration can show a status line using `powerline`. To make this work
you'll need to [install powerline](https://powerline.readthedocs.io/en/latest/installation/linux.html)
The DejaVu Sans Mono font in the `fonts`
directory has been patched to include the Powerline fonts [(see Nerd
Fonts)](https://github.com/ryanoasis/nerd-fonts).If you want to use this
configuration, you'll need to install it. Add the contents of the fonts
directory to your local fonts and then add the new fonts to the font cache,
e.g.

```
$ cp ~/.tmux/fonts/* ~/.local/share/fonts
$ fc-cache ~/.local/share/fonts
```


The `powerline` directory contains my configuration for the `tmux` status line.
If you only use `powerline` for `tmux`, you can just add a link to this
directory in your `.config` directory.

``` shell-session
$ ln -s ~/.tmux/powerline ~/.config/powerline
```

If you already have a `powerline` configuration, you just need to replace
its `tmux` theme with `~/.tmux/powerline/themes/tmux`.
