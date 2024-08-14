# My dotfiles

This directory contains the dotfiles for my system

## Requirements

Ensure you have the following installed on your system

### Git 
```
brew install git
```

### Stow

```
brew install stow
```

## Installation

First, check out the  dotfiles repo in your $HOME directory using git

```
$git clone git@github.com/LuizFmdr/dotfiles.git
$ cd dotfiles
```

then use stow to create symlinks

```
$ stow .
```

# Other Mac settings

## Finder

### Settings -> General 

- [x] Hard disks

New Finder windows show: User folder

### Settings -> SiderBar

- [x] Home folder
- [ ] Tags

### Settings -> Advanced

- [x] Show all filename extensions

When performing a search: search the current folder

### View
- [x] Show Path Bar
- [x] Show Status Bar

## Dock

Minimize windows using 'Scale effect'

- [x] Automatically hide and show the Dock

- [ ] Show suggested and recent apps in Dock

𝗙𝗮𝘀𝘁𝗲𝗿 𝗗𝗼𝗰𝗸 𝗛𝗶𝗱𝗶𝗻𝗴: defaults write com.apple.dock autohide-delay -float 0; defaults write com.apple.dock autohide-time-modifier -int 0;killall Dock
𝗙𝗮𝘀𝘁𝗲𝗿 𝗗𝗼𝗰𝗸 𝗛𝗶𝗱𝗶𝗻𝗴 𝗨𝗻𝗱𝗼: defaults write com.apple.dock autohide-delay -float 0.5; defaults write com.apple.dock autohide-time-modifier -int 0.5 ;killall Dock

𝗔𝗱𝗱 𝗗𝗼𝗰𝗸 𝗦𝗽𝗮𝗰𝗲𝗿 (paste for each spacer): defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}' && killall Dock
𝗔𝗱𝗱 𝗛𝗮𝗹𝗳-𝗛𝗲𝗶𝗴𝗵𝘁 𝗗𝗼𝗰𝗸 𝗦𝗽𝗮𝗰𝗲𝗿 (paste for each): defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="small-spacer-tile";}' && killall Dock

## Screenshot

𝗖𝗵𝗮𝗻𝗴𝗲 𝗦𝗰𝗿𝗲𝗲𝗻𝘀𝗵𝗼𝘁 𝗗𝗲𝗳𝗮𝘂𝗹𝘁 𝘁𝗼 𝗝𝗣𝗚 (replace with png to undo): defaults write com.apple.screencapture type jpg

Keyboard -> Keyboard shortcuts -> Screenshots -> copy picture of selected area to the clipboard = Shit + Command + S

## Hot Corners

Bottom left -> Desktop
