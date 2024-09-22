# Brewfile Initial Setup Configuration
Brewfile configuration for an initial setup on MacOS or Linux using Homebrew.

## Requirements
- Homebrew (install [here](https://brew.sh/))
- MacOS or Linux only

## Installation
```zsh
git clone https://github.com/branzdev/macos-brewfile-config.git
cd macos-brewfile-config
brew bundle install --file ./Brewfile
cd ..
rm -rf macos-brewfile-config
```
Install and upgrade (by default) all dependencies from the Brewfile.

## References
### Homebrew Bundle
- https://github.com/Homebrew/homebrew-bundle

### mas-cli
- https://github.com/mas-cli/mas

Based on the documentation from mas-cli, it's required to have the apps previously purchased and associated with our Apple ID, given that mas-cli is not able to install or purchase an app for the first time.

## Disable MacOS dock animation

```zsh
defaults write com.apple.dock autohide -bool true
defaults write com.apple.dock autohide-time-modifier -int 0
defaults write com.apple.dock autohide-delay -int 0
killall Dock
```

## Restore MacOS dock default behavior

```zsh
defaults write com.apple.dock autohide -bool false
defaults delete com.apple.dock autohide-time-modifier
defaults delete com.apple.dock autohide-delay
killall Dock
```
