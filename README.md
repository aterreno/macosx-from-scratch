###### Install xcode:

	sudo xcodebuild -license	

###### Oh my zsh:

	sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"	

###### Install brew:

	/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
	brew doctor

	Note: if something goes wrong while cloning this should fix it
	git clone https://github.com/Homebrew/homebrew-core /usr/local/Homebrew/Library/Taps/homebrew/homebrew-core --depth=1
	
###### Brewable bare mininum:	

```
brew bundle
dockutil --remove all
	
```
####### powerlevel10k is an excellent theme/extension to zsh
``` 
brew install romkatv/powerlevel10k/powerlevel10k
echo "source $(brew --prefix)/opt/powerlevel10k/powerlevel10k.zsh-theme" >>~/.zshrc
```

###### dev bare mininum (new iterm window):	
```
append to ~/.zshrc 

export NVM_DIR="$HOME/.nvm"
[ -s "/usr/local/opt/nvm/nvm.sh" ] && . "/usr/local/opt/nvm/nvm.sh"  # This loads nvm
[ -s "/usr/local/opt/nvm/etc/bash_completion.d/nvm" ] && . "/usr/local/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion

source  ~/.zshrc 

nvm install node

```
###### Git setup:

	ssh-keygen -t rsa -C "antonio.terreno@example.com"
	eval "$(ssh-agent -s)"
	ssh-add ~/.ssh/id_rsa
	pbcopy < ~/.ssh/id_rsa.pub	
	curl -L https://gist.githubusercontent.com/aterreno/5219929/raw/a9558ef3357c3d7ea730b67fe411fe9313d307d3/.gitconfig > ~/.gitconfig
	vi ~/.gitconfig
	curl -L https://gist.githubusercontent.com/aterreno/5134044/raw/d31e8ca14eb895e77a85652da3869dc29af38f8a/.gitignore > ~/.gitignore 
	vi ~/.gitignore
	
	
###### Vim setup:

	mkdir -p ~/.vim/autoload ~/.vim/bundle && \
	curl -LSso ~/.vim/autoload/pathogen.vim https://tpo.pe/pathogen.vim
	vim ~/.vimrc
	execute pathogen#infect()
	syntax on
	filetype plugin indent on
	cd ~/.vim/bundle && \
	git clone https://github.com/tpope/vim-sensible.git && \
	git clone https://github.com/hashivim/vim-terraform.git && \
	git clone https://github.com/hashivim/vim-packer.git && \
	git clone https://github.com/hashivim/vim-vagrant.git && \
	git clone https://github.com/moll/vim-node && \
	git clone https://github.com/vim-ruby/vim-ruby && \
	git clone https://github.com/ekalinin/Dockerfile.vim.git Dockerfile && \
	git clone --recursive https://github.com/davidhalter/jedi-vim.git && \
	git clone https://github.com/powerline/powerline.git && \
	git clone git://github.com/godlygeek/tabular.git && \ 
	git clone git://github.com/tpope/vim-surround.git && \
	git clone https://github.com/vim-airline/vim-airline.git && \
	git clone https://github.com/elzr/vim-json.git && \ 
	git clone https://github.com/plasticboy/vim-markdown.git && \ 
	git clone git://github.com/tpope/vim-commentary.git && \
	git clone https://github.com/scrooloose/nerdtree.git
