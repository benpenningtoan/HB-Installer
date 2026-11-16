# HB-Installer
Homebrew installer with no permissions required

```
mkdir -p "$HOME/homebrew"
curl -L https://github.com/Homebrew/brew/tarball/main | tar xz --strip 1 -C "$HOME/homebrew"
eval "$("$HOME/homebrew/bin/brew" shellenv)"
echo 'eval "$("$HOME/homebrew/bin/brew" shellenv)"' >> ~/.zshrc
brew update
brew install python
echo 'export PATH="$(brew --prefix python)/libexec/bin:$PATH"' >> ~/.zshrc
export PATH="$(brew --prefix python)/libexec/bin:$PATH"
python --version
python -m pip --version
```
