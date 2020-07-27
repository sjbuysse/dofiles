# dotfiles
To install run                                                                                                                                                        
```
git clone https://github.com/sjbuysse/dotfiles ~/dotfiles
```

If you still need to install vim, make sure it's compiled with python support to be able to install YouCompleteMe.    
You could get the pi-rho PPA repository where vim always has python support.  
 
Delete current .vim folder and .vimrc file, run in homefolder    
```
rm -rf .vim/  
rm -rf .vimrc  
```
Make symbolic links for vim and tmux, run in homefolder  
```
ln -s dotfiles/.vim/  
ln -s dotfiles/.vimrc  
ln -s dotfiles/.ideavimrc  
ln -s dotfiles/.tmux.conf  
```
to make xmledit work for htmlfiles:  
after installing  
```
cd ~/.vim/bundle/xmledit/ftplugin  
rm html.vim  
ln -s xml.vim html.vim  
```
Install plugins using *vundle*, open vim  
```
vim  
```
run the command  
```
:PluginInstall  
```
To compile and install YMC, do the following  
Install development tools and CMake:   
```
sudo apt-get install build-essential cmake  
```
Make sure you have Python headers installed:   
```
sudo apt-get install python-dev   
```
If you want JavaScript autocompletion you have to compile YCM with the '--tern-completer' option  
for this you need to install nodejs and npm  
```
sudo apt-get install nodejs npm  
```
Install YMC  
```
cd ~/.vim/bundle/YouCompleteMe  
./install.sh --tern-completer  
```

# On mac  
=> git clone https://github.com/sjbuysse/dotfiles ~/dotfiles  

If you still need to install vim, make sure it's compiled with python support to be able to install YouCompleteMe  
You could get the pi-rho PPA repository where vim always has python support  
 
Delete current .vim folder and .vimrc file, run in homefolder
```
rm -rf .vim/  
rm -rf .vimrc  
```
Make symbolic links for vim and tmux, run in homefolder   
```
ln -s dotfiles/.vim/
ln -s dotfiles/.vimrc
ln -s dotfiles/.tmux.conf
```

Install macvim met brew (zodat YMC kan werken)   
```
brew install macvim
```
maak een alias aan voor mvim  
```
echo "alias vim='mvim -v'" > ˜/.bash_profile 
```
Install plugins using *vundle*, open vim  
```
vim
```
run the command in vim
```
:PluginInstall
```

to make xmledit work for htmlfiles:  
after installing  
```
cd ~/.vim/bundle/xmledit/ftplugin
rm html.vim
ln -s xml.vim html.vim
```
To compile and install YMC, do the following  
Install development tools and CMake:   
```
brew install cmake
```
If you want JavaScript autocompletion you have to compile YCM with the `--tern-completer` option   
for this you need to install nodejs and npm
```
brew install node
```
Install YMC
```
cd ~/.vim/bundle/YouCompleteMe
./install.sh --tern-completer
```

