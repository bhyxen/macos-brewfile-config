# MacOS Brewfile Initial Setup Configuration
Brewfile configuration for an initial setup on MacOS using Homebrew.

## Installation
```console
git clone git@github.com:bmongemendez/macos-brewfile-config.git
cd macos-brewfile-config
sudo brew bundle install --file ./Brewfile
```
Install and upgrade (by default) all dependencies from the Brewfile.

## References:
### Homebrew Bundle
- https://github.com/Homebrew/homebrew-bundle

### mas-cli
- https://github.com/mas-cli/mas

Based on the documentation from mas-cli, it is required to have the apps previously purchased and associated with our Apple ID, given that mas-cli is not able to install or purchase an app for the first time.
