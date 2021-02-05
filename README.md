# Mac from scatch

## Install xcode

`sudo xcodebuild -license`

## Oh my zsh

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

## Install brew

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/§install)"

brew doctor
```

### Brewable bare mininum

```bash
brew bundle
```

Remove all default icons in the dock:

```bash
dockutil --remove all
```

## powerlevel10k is an excellent theme/extension to zsh

```bash
brew install romkatv/powerlevel10k/powerlevel10k`
echo "source $(brew --prefix)/opt/powerlevel10k/powerlevel10k.zsh-theme" >>~/.zshrc`
```

## dev bare mininum (new iterm window)

append to ~/.zshrc nvm and install latest node version

```bash
export NVM_DIR="$HOME/.nvm"
[ -s "/usr/local/opt/nvm/nvm.sh" ] && . "/usr/local/opt/nvm/nvm.sh" # This loads nvm
[ -s "/usr/local/opt/nvm/etc/bash_completion.d/nvm" ] && . "/usr/local/opt/nvm/etc/bash_completion.d/nvm" # This loads nvm bash_completion
source ~/.zshrc
nvm install node
```
append to ~/.zshrc autojump (can be called with a j) 
  ```bash
  [ -f /usr/local/etc/profile.d/autojump.sh ] && . /usr/local/etc/profile.d/autojump.sh
  ```

## Git setup

```bash
    ssh-keygen -t rsa -C "antonio.terreno@example.com"
    eval "$(ssh-agent -s)"
    ssh-add ~/.ssh/id_rsa
    pbcopy < ~/.ssh/id_rsa.pub
    curl -L https://gist.githubusercontent.com/aterreno/5219929/raw/cc8fcbf5a6a496de381c7124d0e21cc241f87843/.gitconfig > ~/.gitconfig
    vi ~/.gitconfig
    curl -L https://gist.githubusercontent.com/aterreno/5134044/raw/d31e8ca14eb895e77a85652da3869dc29af38f8a/.gitignore > ~/.gitignore
    vi ~/.gitignore
```

## Vim setup

```bash
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
```
