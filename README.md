###### Oh my zsh:

	curl -L http://install.ohmyz.sh | sh
	vi ~/.zshrc
	
###### Install xcode:

	sudo xcodebuild -license	
	xcode-select --install    

###### Install brew:

	ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
	brew doctor


###### Install rvm&ruby:
	
	brew install gpg
	gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
	\curl -sSL https://get.rvm.io | bash -s stable --ruby
	
###### Install nvm&node:	

	curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.29.0/install.sh | bash
	nvm alias default stable

###### Brewable bare mininum:	

```
brew cask install atom
brew cask install caffeine
brew cask install dropbox
brew cask install evernote
brew cask install firefox
brew cask install google-chrome 
brew cask install google-drive
brew cask install iterm2
brew cask install kindle
brew cask install mou
brew cask install omnigraffle
brew cask install skype
brew cask install slack
brew cask install spectacle
brew cask install spotify
brew cask install sublime-text3
brew cask install the-unarchiver
brew cask install utorrent
brew cask install virtualbox
brew install caskroom/cask/brew-cask
brew install docker
brew install dockutil
brew install elixir
brew install emacs --HEAD --use-git-head --cocoa
brew install git
brew install git-extras
brew install git-flow
brew install leiningen	
brew install macvim
brew install picasa
dockutil --remove all
```
###### Brewable dev bare mininum:	
```
brew install apache2
brew install rabbitmq
brew install mysql
brew install graphviz
brew install aspell
brew install java
brew install rubymine
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

###### Internet explorer virtual machines (for the braves):

	curl -O "https://az412801.vo.msecnd.net/vhd/IEKitV1_Final/VirtualBox/OSX/IE8_XP/IE8.XP.For.MacVirtualBox.ova"
	curl -O "https://az412801.vo.msecnd.net/vhd/IEKitV1_Final/VirtualBox/OSX/IE9_Win7/IE9.Win7.For.MacVirtualBox.part{1.sfx,2.rar,3.rar,4.rar,5.rar}"
	curl -O "https://az412801.vo.msecnd.net/vhd/IEKitV1_Final/VirtualBox/OSX/IE10_Win8/IE10.Win8.For.MacVirtualBox.part{1.sfx,2.rar,3.rar}"
	brew cask install iterm2-beta
