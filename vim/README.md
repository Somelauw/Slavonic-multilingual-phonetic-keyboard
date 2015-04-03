[Vim](http://www.vim.org/) is a popular text editor among programmers.
The file russian.vim assist Vim users by making common keybindings available
again when using this keyboard layout.

##Instructions
Put the file russian.vim in $HOME/.vim/plugin

This will make common keybinding like dd, yy, h, j, k, l work in normal and visual mode.
However for complexer keybindings like da10w you'll still need to switch to an English keyboard.

##xkblayout-state
If you want to make other keybindings available as well, 
clone and install https://github.com/nonpop/xkblayout-state

Put this command in your .vimrc

    autocmd InsertLeave * :!xkblayout-state set 0

This will make it so that whenever you leave insert mode, your keyboard layout is automatically switched to the default one (which is probably English).
Whether that's desirable is probably a matter of preference.

