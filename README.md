# HB-Installer
Homebrew installer with no permissions required

```
mkdir ~/homebrew && curl -L https://github.com/Homebrew/brew/tarball/main | tar xz --strip 1 -C ~/homebrew
brew update --force --quiet
chmod -R go-w "$(brew --prefix)/share/zsh"
echo 'eval "$(~/hb/bin/brew shellenv)"' >> ~/.zshrc
source ~/.zshrc
brew install pip python python3
python -m pip --version
```
