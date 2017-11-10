# Vim 설정
'~/.vimrc' 파일에 입력 내용

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

	autocmd FileType python setlocal completeopt-=preview
