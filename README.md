```
brew install git
brew install caskroom/cask/brew-cask
brew install docker
brew install node
brew install macvim
brew install ruby
brew install rvm
brew install nvm
brew tap caskroom/versions
brew update
brew cask install evernote
brew cask install spectacle
brew cask install iterm2
brew cask install slack
brew cask install sublime-text3
brew cask install dropbox
brew cask install omnigraffle
brew cask install sublime-text
brew cask install skype
brew cask install spotify
brew cask install virtualbox
brew cask install mou
brew cask install utorrent
brew cask install firefox
brew cask install spectacle
brew cask install caffeine
brew cask install the-unarchiver
brew cask install google-chrome google-drive
brew search dockutil
brew install dockutil
dockutil --remove all
   30  brew search dockutil
   31  brew install dockutil
   35  vi brew.sh 
   39  brew cask search kuvva
   40  brew cask search kindle
   41  brew cask install kindle
   42  brew cask search picasa
   43  brew install picasa
   45  brew search atom
   59  brew install atom
   60  brew update
   62  brew update
   63  brew install atom
   64  brew cask install atom
   66  brew info postgresql
   87  brew install elixir
   92  brew install postgres
```

###### Install xcode:

	sudo xcodebuild -license	
	xcode-select --install    

###### Install brew:

	ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
	
	brew doctor
	
###### Git setup:

	ssh-keygen -t rsa -C "antonio.terreno@example.com"
	eval "$(ssh-agent -s)"
	ssh-add ~/.ssh/id_rsa
	pbcopy < ~/.ssh/id_rsa.pub	
	curl -L https://gist.githubusercontent.com/aterreno/5219929/raw/a9558ef3357c3d7ea730b67fe411fe9313d307d3/.gitconfig > ~/.gitconfig
	vi ~/.gitconfig
	curl -L https://gist.githubusercontent.com/aterreno/5134044/raw/d31e8ca14eb895e77a85652da3869dc29af38f8a/.gitignore > ~/.gitignore 
	vi ~/.gitignore
	
###### Oh my zsh:

	curl -L http://install.ohmyz.sh | sh
	vi ~/.zshrc

###### Brewable software: 

	brew install git
	brew install git-extras
	brew install leiningen
	brew install caskroom/cask/brew-cask
	brew install emacs --HEAD --use-git-head --cocoa
	brew install git-flow

###### Brewable (with cask) software: 	
	
	brew tap caskroom/versions
	brew update
	brew cask install airfoil	
	brew cask install dropbox
	brew cask install garmin-express
	brew cask install omnigraffle
	brew cask install sublime-text
	brew cask install skype
	brew cask install spotify
	brew cask install virtualbox
	brew cask install mou
	brew cask install utorrent
	brew cask install firefox
	brew cask install spectacle
	brew cask install caffeine
	brew cask install the-unarchiver

###### Internet explorer virtual machines:

	curl -O "https://az412801.vo.msecnd.net/vhd/IEKitV1_Final/VirtualBox/OSX/IE8_XP/IE8.XP.For.MacVirtualBox.ova"
	curl -O "https://az412801.vo.msecnd.net/vhd/IEKitV1_Final/VirtualBox/OSX/IE9_Win7/IE9.Win7.For.MacVirtualBox.part{1.sfx,2.rar,3.rar,4.rar,5.rar}"
	curl -O "https://az412801.vo.msecnd.net/vhd/IEKitV1_Final/VirtualBox/OSX/IE10_Win8/IE10.Win8.For.MacVirtualBox.part{1.sfx,2.rar,3.rar}"
	brew cask install iterm2-beta
	

