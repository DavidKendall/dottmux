# dottmux
A simple tmux configuration that uses 
a [onedark theme](https://github.com/bk2dcradle/dotfiles/blob/master/tmux/themes/tmux.onedark.sh)

# Installation

``` shell-session
$ cd ~
$ git clone https://github.com/DavidKendall/dottmux.git ~/.tmux
$ ln -s ~/.tmux/tmux.conf ~/.tmux.conf
```
# Use
I like to run `tmux` in an `xterm`. If you want to use
this configuratin, you'll need to install it and configure your `.Xresources` file, based on
`Xresources`.  (If you don't already have a `.Xresources` file, you can just
copy `Xresources` to `~\.Xresources`). See [this
note](http://www.futurile.net/2016/06/14/xterm-setup-and-truetype-font-configuration/)
for guidance on configuring `xterm`.

