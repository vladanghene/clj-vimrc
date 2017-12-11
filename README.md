# vlad-vimrc
## a clojurian vim that feels nice and has all the coveted plugins: fireplace, autoindent, etc. and some of my personal faves : navigating between buffers and showing 80-line bar

Use these commands to setup your vim editor

First install [PlugInstall](https://github.com/junegunn/vim-plug)
In order to do this, download plug.vim and put it in the "autoload" directory.


```bash
mkdir ~/.vim/autoload && cd ~/.vim/autoload
wget https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

After that, run these commands to update your .vimrc to point to clj-vimrc's and to install all needed plugins and powerline
Then you'll have it all and it should enter with default colorscheme=gruvbox

```bash
ln -s clj-vimrc/.vimrc ~/.vimrc
vim +PlugInstall +qall
cd ~/.vim/plugged/vimproc.vim && make
pip install --user git+git://github.com/Lokaltog/powerline
```
