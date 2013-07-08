## Installation:
    * Need to install `exuberant-ctags`
    * Need to install `vim-gtk` or equivalent for 256 color schemes
    
    apt-get install exuberant-ctags vim-gtk

    Now clone the repo
    git clone https://github.com/ProggyBS/dotfiles.git ~/.dotfiles

## Create symlinks:

    ln -s ~/.dotfiles/.vim ~/.vim
    ln -s ~/.dotfiles/.vim/.vimrc ~/.vimrc
    ln -s ~/.dotfiles/.bash_aliases ~/.bash_aliases
    ln -s ~/.dotfiles/.bashrc ~/.bashrc
    ln -s ~/.dotfiles/.gemrc ~/.gemrc
    ln -s ~/.dotfiles/.irbrc ~/.irbrc
    ln -s ~/.dotfiles/.screenrc ~/.screenrc

## Switch to the `~/.dotfiles` directory, and fetch submodules:

    cd ~/.dotfiles
    git submodule init
    git submodule update

## Upgrading all bundled plugins
    
  `git submodule foreach git pull origin master`

## Adding plugins

    cd ~/.vim
    git submodule init
    git submodule add git://github.com/foo/bar.git bundle/vim-foo
    git commit -m 'Added vim-foo'
    git push origin master
