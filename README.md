# vlad-vimrc
## a clojurian vim that feels nice and has all the coveted plugins: fireplace, autoindent, etc. and some of my personal faves : navigating between buffers and showing 80-line bar

Use these commands to setup your vim editor

### Obviously, first clone this repo in your home folder (or where ever, but make sure to update the below link path).


First install [PlugInstall](https://github.com/junegunn/vim-plug)
In order to do this, download plug.vim and put it in the "autoload" directory.


```bash
mkdir ~/.vim/autoload && cd ~/.vim/autoload
wget https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

After that, run these commands to update your .vimrc to point to clj-vimrc's and to install all needed plugins and powerline

```bash
ln -s clj-vimrc/.vimrc ~/.vimrc
vim +PlugInstall +qall
```
Make sure you have binutils and gcc for this one:

```
cd ~/.vim/plugged/vimproc.vim && make
pip install --user git+git://github.com/Lokaltog/powerline
```

Finally, you'll have it all and it should enter with default colorscheme=gruvbox


# Font I recommend #
For *bonus points*. 
Make sure to get yourself [Inconsolata](https://github.com/cyrealtype/Inconsolata/tree/master/fonts/otf). 
Save those two files in .fonts dir or `mkdir ~/.fonts && cd ~/.fonts` if you have no .fonts folder. Next:

```
wget https://github.com/cyrealtype/Inconsolata/blob/master/fonts/otf/Inconsolata-Bold.otf
wget https://github.com/cyrealtype/Inconsolata/blob/master/fonts/otf/Inconsolata-Regular.otf
```

After this run a 
```
sudo fc-cache -v
```

There ya go ! Now you have gvim (which enables os clipboard so you can paste in other apps --- as opposed to classic vim) which looks great and has lotsa funcionality. Enjoy. Star me if you think this helped you.
