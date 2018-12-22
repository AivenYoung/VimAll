# VimAll

## The version of VIM should >= 8.0 or else some tools related will not work functionly. The plugins I collected are C/C++ oriented and I do not have a mind if others languages is suitable.

## Necessary Softwares
* [VIM](https://github.com/vim/vim)
The version of VIM comes with the System may be too old. We can reinstall it by the latest source code.

* [GNU GLOBAL](http://www.gnu.org/software/global/download.html)
The latest version of gtags canbe acheived at the website above.
Gtags should be installed by source code or using the command __ sudo apt install gtags __.
We should copy __"gtags.vim"__ and  __"gtags_cscope.vim"__ from directory __"/usr/local/share/gtags/"__ to __"~/.vim/plugin/"__ so that we can use gtags properly.


## Plugins
* The "plugin.vim" is prepared in directory ".vim/plugin". All other plugin scripts will be auto-loaded by performing __":PlugInstall"__ in VIM. 

* The color-scheme I used is "molokai" which defined in __"~/.vim/colors/molokai.vim"__. 

* The plugin named vim-airline status line will not be displayed normally until the specified patched fonts being used. After performing __":PlugInstall"__, you can find valid fonts in dirctory __"~/.vim/plugged/fonts"__.

* YouCompleteMe will also be auto-loaded by __":PlugInstall"__ but not installed totally. You can install it according to the NOTE at the website [YouCompleteMe](https://github.com/Valloric/YouCompleteMe).

	The configuration file __".vim/.ycm_extra_conf.py"__ is prepared for YouCompleteMe. ___C++/C header directory___ of my own has been added to it but not yours. You should modify the file according to your system.
	Note: clang dev and llvm dev librarys should be installed at first  according to the website.

## \.vim directory and files
```
.
├── autoload
│   └── plug.vim
├── colors
│   └── molokai.vim
├── plugged
│   ├── DoxygenToolkit.vim
│   ├── TaskList.vim
│   ├── YouCompleteMe
│   ├── a.vim
│   ├── ale
│   ├── auto-pairs
│   ├── bufexplorer.zip
│   ├── command-t
│   ├── ctrlp-funky
│   ├── ctrlp.vim
│   ├── gutentags_plus
│   ├── indentLine
│   ├── minibufexpl.vim
│   ├── molokai
│   ├── nerdcommenter
│   ├── nerdtree
│   ├── rainbow_parentheses.vim
│   ├── tabular
│   ├── taglist.vim
│   ├── vim-airline
│   ├── vim-airline-themes
│   ├── vim-autoformat
│   ├── vim-cpp-enhanced-highlight
│   ├── vim-easymotion
│   ├── vim-fugitive
│   ├── vim-gutentags
│   ├── vim-mark
│   └── vim-preview
└── plugin
    ├── gtags-cscope.vim
    └── gtags.vim

```
