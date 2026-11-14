# HB-Installer
Homebrew installer with no permissions required

```
mkdir homebrew && curl -L https://github.com/Homebrew/brew/tarball/main | tar xz --strip 1 -C homebrew
echo $'eval "$(~/hb/bin/brew shellenv)"\n\n# Created by `pipx` on 2026-09-25 13:17:55\nexport PATH="$PATH:~/.local/bin"' >.zshrc
```
