#Ubuntu-VIM Setting
If you want Korean Ver, click [English Ver]()
##Vim shortcut
/ : Search
Ctrl + W : move viewport
##Vim Setting
write below settings on '/.vimrc' file
	""Setting
	let python_version_2 = 1
	let python_highlight_all = 1
	syntax on
	set tabstop=8
	set expandtab
	set softtabstop=4
	set autoindent
	set bg=dark
	set nu
	set hlsearch
	""Plugin
	set rtp+=~/.vim/bundle/Vundle.vim
	call vundle#begin()
	Plugin 'VundleVim/Vundle.vim'
	Plugin 'AutoComplPop'
	Plugin 'The-NERD-tree'
	Plugin 'jedi-vim'
	Plugin 'delimitMate.vim'
	call vundle#end()
	filetype indent plugin on

	autocmd FileType python setlocal completeopt-=preview "remove docstring part in jedi-vim

##Plugin 
Must write plugin part as above '~/.vimrc'.
###Vundle
Using Vundle, can search & install Vim plugin.
####1. Installation
Download source using git,
	git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
If git is not installed,
	sudo apt-get install git
####2. Use
After excuting vim, can search&install plugins by ':BundleSearch'.

###AutoComplPop
Auto completion plugin.
####1. Installation
Using Vundle, search 'AutocomplPop' and install.

###The-NERD-tree
File Directory plugin.
####1. Installation
Using Vundle, search 'The-NERD-tree' and install.
####2. Use
Excute File Directory by ':NERDTree'.

###jedi-vim
module function auto completion plugin.
####1. Installation
download source using git.
	git clone --recursive https://github.com/davidhalter/jedi-vim.git ~/.vim/bundle/jedi-vim
* Refer to [github page](https://github.com/davidhalter/jedi-vim).
####2. Use
Show list of completions by 'Ctrl+Space'.
It takes time to save in cache at first time.

###delimitMate
Brackets auto completion plugin.
####1. Installation
Using Vundle, search 'delimitMate.vim' and install.
