# vlad-vimrc
## my vim config

Use these commands to setup your vim editor

vim +PlugInstall +qall
cd ~/.vim/plugged/vimproc.vim && make
pip install --user git+git://github.com/Lokaltog/powerline

## Installation

Download plug.vim and put it in the "autoload" directory.
Unix

curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
