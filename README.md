# Mac OS X setup
Facing the setup of a new machine (or the need to reinstall after a fresh OS install or the like), here's a very brief and basic list of the usual suspects, related to the setup of a mac computer to work with (mostly related to a scripting languages context).

## Homebrew & Cask
The package manager is the default first thing I always install. Simply following the default steps. Homebrew downloads and installs the Command Line Tools for Xcode, so we're all good. Homebrew Cask is implemented as part of Homebrew now, so we're cask-enabled and ready from the start for our tapping. Finally, `brew-cask-upgrade` provides upgrade-like capabilities to cask, and we're all set.

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew tap buo/cask-upgrade

## Mac App Store
If some previously purchased software from the Mac App Store needs to be included, we can use `mas` to ease the installs.

brew install mas

## My curated list of apps (and all that jazz)
Once we have `homebrew`, `cask` (and `mas` if needed) we're ready to go (and yes, these lists might be scripted for some automation to install all, take this as just a curated set):

### Productivity

# Slack
brew install slack

# Notes & related
mas install 1091189122 #Bear
brew install evernote
brew install notion
brew install obsidian
brew install skitch
brew install typora

# Amphetamine
mas install 937984704

# Browsers
brew install microsoft-edge

### Common apps

# Authy
brew install authy

# Personal cloud storage
brew install dropbox

# MS
brew install microsoft-office

# VLC
brew install vlc

# Videoconference
brew install microsoft-teams
brew install zoom

# Messaging
brew install signal

### Development

# A good terminal
brew install iterm2
brew install tree
brew install wget

# AWS CLI
brew install awscli

# API development
brew install paw
brew install postman

# Text editors/IDEs
brew install sublime-text

# Charles proxy
brew install charles

# Cloud storage and related
brew install cyberduck
brew install mountain-duck
brew install duck


# VPN
brew install tunnelblick

# Xcode. Will take forever to download, yes. Not needed by everyone.
mas install 497799835
