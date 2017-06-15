# dotfiles
To install run                                                                                                                                                        
=> git clone https://github.com/sjbuysse/dotfiles ~/dotfiles
 
Delete current .vim folder and .vimrc file, run in homefolder
=> rm -rf .vim/
=> rm -rf .vimrc
Make symbolic links for vim and tmux, run in homefolder
=> ln -s dotfiles/.vim/
=> ln -s dotfiles/.vimrc
=> ln -s dotfiles/.tmux.conf

to make xmledit work for htmlfiles:
after installing
=> cd ~/.vim/xmledit/ftplugin
=> rm html.vim
=>ln -s xml.vim html.vim

Install plugins using vundle, open vim
=> vim
run the command
=> :PluginInstall

To compile and install YMC, do the following
Install development tools and CMake: 
=> sudo apt-get install build-essential cmake
Make sure you have Python headers installed: 
=> sudo apt-get install python-dev
Install YMC
=> cd ~/.vim/bundle/YouCompleteMe
=> ./install.sh
