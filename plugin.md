
Vim 설정의 '~/.vimrc'와 같이 ""Plugin 부분 입력해야 사용 가능

[plugin 참조](https://agvim.wordpress.com/2017/09/05/vim-plugins-50/)

# Vundle: Vim plugin 검색 및 설치 plugin
 ### 설치 방법
git으로 다운받기

	git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
	
git 설치 안되어 있으면,

	sudo apt-get install git
	
 ### 사용법
vim실행 후, ':BundleSearch'입력하면 plugin 검색&설치 가능

# AutoComplPop: 자동완성 plugin
### 설치 방법
Vundle 로 'AutocomplPop' 검색 후 설치

# The-NERD-tree: 파일 탐색기 plugin
### 설치 방법
Vundle로 'The-NERD-tree' 검색 후 설치
### 사용법
':NERDTree' 입력하면 파일 탐색기 실행

# jedi-vim: module 함수 자동완성 plugin
### 설치 방법
git으로 다운받기

	git clone --recursive https://github.com/davidhalter/jedi-vim.git ~/.vim/bundle/jedi-vim
	
* [github 홈페이지](https://github.com/davidhalter/jedi-vim) 참조
### 사용법
'Ctrl+Space'누르면 자동 완성 목록 보기
단점) 맨 처음 검색시에만 캐시에 저장하느라 시간이 조금 걸림

# delimitMate: 괄호 자동 완성 플러그인
### 설치 방법
Vundle로 'delimitMate.vim' 검색 후 설치
