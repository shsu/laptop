#!/usr/bin/env bash

brew_install_or_upgrade 'coreutils'
append_to_zshrc 'export PATH="/usr/local/opt/coreutils/libexec/gnubin:$PATH"'
append_to_zshrc 'export MANPATH="/usr/local/opt/coreutils/libexec/gnubin:$MANPATH"'

brew_install_or_upgrade 'moreutils'
sudo ln -s /usr/local/bin/gsha256sum /usr/local/bin/sha256sum

brew_install_or_upgrade 'findutils'

brew install gnu-sed --with-default-names
append_to_zshrc 'export PATH="/usr/local/opt/gnu-sed/libexec/gnubin:$PATH"'
append_to_zshrc 'export MANPATH="/usr/local/opt/gnu-sed/libexec/gnubin:$MANPATH"'

brew_install_or_upgrade 'bash'
brew_install_or_upgrade 'bash-completion'

# Install wget with IRI support
brew install wget --with-iri

# Install more recent versions of some OS X tools
brew install vim --override-system-vi
brew tap homebrew/dupes
brew_install_or_upgrade 'homebrew/dupes/grep'
brew_install_or_upgrade 'homebrew/dupes/screen'

# Install some CTF tools; see https://github.com/ctfs/write-ups
brew_install_or_upgrade 'nmap'

# Install other useful binaries
brew_install_or_upgrade 'ack'
brew_install_or_upgrade 'git'
brew_install_or_upgrade 'p7zip'
brew_install_or_upgrade 'pigz'
brew_install_or_upgrade 'pv'
brew_install_or_upgrade 'rename'
brew_install_or_upgrade 'sqlmap'
brew_install_or_upgrade 'tree'

# Thoughtbot laptop stuff
brew_install_or_upgrade 'gh'
brew_install_or_upgrade 'imagemagick'
brew_install_or_upgrade 'qt'
brew_install_or_upgrade 'the_silver_searcher'
brew_install_or_upgrade 'watch'

# zsh additions
brew_install_or_upgrade 'zsh'
brew_install_or_upgrade 'zsh-syntax-highlighting'
append_to_zshrc 'source /usr/local/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh'

# docker stuff
brew_install_or_upgrade 'docker'
brew_install_or_upgrade 'boot2docker'

# Remove outdated versions from the cellar
brew cleanup
