Jair's vimrc
============
Forked form https://github.com/vgod/vimrc.

Installation
----------------

     curl -o - https://raw.github.com/vgod/vimrc/master/auto-install.sh | sh

Manual Installation
----------------

1. Check out from github

        git clone git://github.com/jairzh/vimrc.git ~/.vim
        cd ~/.vim
        git submodule update --init

2. Install ~/.vimrc and ~/.gvimrc

        ./install-vimrc.sh

3. (Optional, if you want Command-T) Compile the Command-T plugin

        cd .vim/bundle/command-t
        rake make

  
Install & Upgrade plugin bundles
--------------------------------

All plugins (except vim-latex) were checked out as git submodules, 
which can be upgraded with `git pull`. For example, to upgrade Command-T 

     cd ~/.vim/bundle/command-t
     git pull

Upgrading all bundled pugins

     git submodule foreach git pull origin master
     git submodule update

To install a new plugin as a git submoudle, type the followin commands.

     cd ~/.vim
     git submodule add [GIT-REPOSITORY-URL] bundle/[PLUGIN-NAME]

Plugins
-------

* [Pathogen](http://www.vim.org/scripts/script.php?script_id=2332)

* [Nerd Tree](http://www.vim.org/scripts/script.php?script_id=1658)

* [AutoClose](http://www.vim.org/scripts/script.php?script_id=1849)

* [vim-surround](https://github.com/tpope/vim-surround/blob/master/doc/surround.txt)

* [matchit](http://www.vim.org/scripts/script.php?script_id=39)

* [xmledit](http://www.vim.org/scripts/script.php?script_id=301)

* [Command-T](https://github.com/wincent/Command-T)
  
* [SuperTab](http://www.vim.org/scripts/script.php?script_id=1643)

* [snipMate](http://www.vim.org/scripts/script.php?script_id=2540)

* [YankRing](http://www.vim.org/scripts/script.php?script_id=1234)

* [VisIncr](http://www.vim.org/scripts/script.php?script_id=670)
  
* [Cute Error Marker](http://www.vim.org/scripts/script.php?script_id=2653)

* [vim-latex](http://vim-latex.sourceforge.net/)

* [OmniCppComplete](http://www.vim.org/scripts/script.php?script_id=1520)

* [JavaComplete](http://www.vim.org/scripts/script.php?script_id=1785)

* [EasyMotion](https://github.com/Lokaltog/vim-easymotion)

* [Ant_menu](https://github.com/vim-scripts/ant_menu.vim)

* [Forcedotcom](https://github.com/ejholmes/vim-forcedotcom)


Language specific supports
--------------------------

* Latex: Read `:help latex-suite.txt`
* Restructured Text: `ctrl-u 1~5` inserts Part/Chapter/Section headers
* HTML, Javascript, Python, CSS, C, C++, Java: use `TAB` to do omni-completion.
* HTML/XML: End tags are automatically completed after typing a begin tag. (Typing > twice pushes the end tag to a new line.)

Other good references
---------------------

* [Synchronizing plugins with git submodules and pathogen](http://vimcasts.org/episodes/synchronizing-plugins-with-git-submodules-and-pathogen/) 
    How to keep your vimrc and plugins synchronized using git submodules and the pathogen plugin

* [spf13-vim : Steve Francia's Vim Distribution](https://github.com/spf13/spf13-vim/tree/master)
