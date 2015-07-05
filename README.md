# dofiles
# dotfiles
To install run
=> git clone https://github.com/sjbuysse/dotfiles ~/dotfiles

Delete current .vim folder and .vimrc file, run in homefolder
=> rm -rf .vim/
=> rm -rf .vimrc
Make symbolic links for vim, run in homefolder
=> ln -s /dotfiles/.vim/
=> ln -s /dotfiles/.vimrc

Install plugins using vundle, open vim
=> vim
run the command
=> :PluginInstall
