# Mac from scatch

## Install xcode

`sudo xcodebuild -license`

## Install Rosetta (if on M1 CPU)

`/usr/sbin/softwareupdate --install-rosetta --agree-to-license`

## Oh my zsh

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

## Install brew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

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
[ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && . "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
[ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && . "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completionsource ~/.zshrc
nvm install node
```
append to ~/.zshrc autojump (can be called with a j) 
  ```bash
  [ -f /opt/homebrew/etc/profile.d/autojump.sh ] && . /opt/homebrew/etc/profile.d/autojump.sh
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

## Add GPG Key 

Follow [this](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-gpg-key) guide

```bash
  gpg --list-secret-keys --keyid-format LONG
  gpg --armor --export <gpg_key_id>  
```

## Vim setup

https://dancroak.com/vim-react-typescript
