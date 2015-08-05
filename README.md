# dofiles
# dotfiles
To install run
=> git clone https://github.com/sjbuysse/dotfiles ~/dotfiles

Make symbolic links for vim, run in homefolder
=> ln -s /dotfiles/.vim/
=> ln -s /dotfiles/.vimrc

Install plugins using vundle, open vim
=> vim
run the command
=> :PluginInstall

To make xmledit work for html tags you should make a symbolic link with the xml settings
=> cd ~/.vim/bundle/xmledit/ftplugin
=> mv html.vim html.vim.bk
=> ln -s xml.vim html.vim 
