###### Install xcode:

	sudo xcodebuild -license	

###### Oh my zsh:

	sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
	vi ~/.zshrc
	

###### Install brew:

	/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
	brew doctor
	
###### Brewable bare mininum:	

```
brew cask install caffeine
brew cask install dropbox
brew cask install evernote
brew cask install firefox
brew cask install google-drive
brew cask install iterm2
brew cask install omnigraffle
brew cask install skype
brew cask install slack
brew cask install spectacle
brew cask install spotify
brew cask install sublime-text
brew cask install the-unarchiver
brew cask install virtualbox
brew cask install tunnelblick
brew cask install avibrazil-rdm
brew cask install screenhero
brew cask install numi
brew cask install intellij-idea
brew install dockutil
brew install git
brew install ansible
brew install autojump
brew install figlet
brew install jq
brew install wget
brew install macvim
brew install nvm
brew install gpg2
brew install tfenv
brew install ccat
dockutil --remove all
curl -s "https://get.sdkman.io" | bash
gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
curl -sSL https://get.rvm.io | bash
	
```
###### dev bare mininum (new iterm window):	
```
sdk install java
sdk install gradle
nvm install node
rvm install ruby
tfenv install 0.9.2
echo "get latest packer & vagrant from hashicorp - no good brew formula yet"

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
	git clone https://github.com/vim-ruby/vim-ruby



###### Internet explorer virtual machines (for the braves):

	curl -O "https://az412801.vo.msecnd.net/vhd/IEKitV1_Final/VirtualBox/OSX/IE8_XP/IE8.XP.For.MacVirtualBox.ova"
	curl -O "https://az412801.vo.msecnd.net/vhd/IEKitV1_Final/VirtualBox/OSX/IE9_Win7/IE9.Win7.For.MacVirtualBox.part{1.sfx,2.rar,3.rar,4.rar,5.rar}"
	curl -O "https://az412801.vo.msecnd.net/vhd/IEKitV1_Final/VirtualBox/OSX/IE10_Win8/IE10.Win8.For.MacVirtualBox.part{1.sfx,2.rar,3.rar}"
