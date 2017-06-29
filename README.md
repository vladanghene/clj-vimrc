# vlad-vimrc
## my vim config

Use these commands to setup your vim editor

First install [PlugInstall](https://github.com/junegunn/vim-plug)
In order to do this, download plug.vim and put it in the "autoload" directory.
Unix

`
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
`

After, run these commands:

`
ln -s vlad-vimrc/.vimrc ~/.vimrc
vim +PlugInstall +qall
cd ~/.vim/plugged/vimproc.vim && make
pip install --user git+git://github.com/Lokaltog/powerline
`
