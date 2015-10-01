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
	
	
	
brew list
autoconf	docker		gradle		libyaml		node
automake	emacs		leiningen	macvim		openssl
boot2docker	fig		libevent	maven		pkg-config
brew-cask	git		libgpg-error	mongodb		postgresql
cmake		git-extras	libksba		mysql		readline
cscope		gnupg		libtool		neo4j
➜  ~  brew cask list
airfoil		    evernote		microsoft-office    pgadmin3		spectacle	    teamviewer		vagrant
caffeine	    garmin-express	mou		    skype		spotify		    the-unarchiver	virtualbox
dropbox		    iterm2		omnigraffle	    slack		sublime-text3	    utorrent		vlc
➜  ~	
