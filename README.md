# setup
Links and preferences for quick setup of personal development environment

## Heavily borrowed from following pages
- Windows - https://scotch.io/tutorials/get-a-functional-and-sleek-console-in-windows
- https://github.com/mdo/config

## Setup Windows
- copy ssh keys from Dropbox to -> users/[username]/.ssh/
- Install [WinSCP](https://winscp.net/eng/download.php) and import settings file from Dropbox
- Install [Node.js](https://nodejs.org/en/) 
- Install [Git](https://git-scm.com/download/win)
- Install [ConEmu](https://conemu.github.io/)
- Choose `{Bash::Git bash}` as startup task on inital launch config
  - If there is error, point startup task to -> program files/git/bin/sh.exe
- Open Settings and Import [`ConEmu.xml`](ConEmu.xml)
- 


## Dev dependencies
- Gulp `npm install -g gulp`

## Brackets 
- Install Brackets [[Link](http://brackets.io/)]
- Install Brackets extensions:
  - Extensions Bulk Installer (use the config file in Dropbox)
- Copy brackets.json file from Dropbox to \Users\[username]\AppData\Roaming\Brackets
- Add EditorConfig file to webdev root

## TTÜ
- Go to -> https://wiki.ttu.ee/it/et/doc/vpn and install the vpn client
- Start vpn and go to https://itwiki.intra.ttu.ee/ to get repo addresses 

## Sublime Text
- Install Sublime Text 3 [[Link](http://www.sublimetext.com/3)]
- Install Package Control [[Link](https://packagecontrol.io/installation)]
- Install packages through Package Control
  - [Predawn](https://github.com/jamiewilson/predawn)
  - [Tomorrow Color Schemes](https://github.com/theymaybecoders/sublime-tomorrow-theme/)
  - [CSS3](https://github.com/y0ssar1an/CSS3)
  - [LESS](https://github.com/danro/LESS-sublime/)
  - [Emmet](https://github.com/sergeche/emmet-sublime/)
  - [GitGutter](https://github.com/jisaacks/GitGutter)
  - [SidebarEnhancements](https://github.com/titoBouzout/SideBarEnhancements)
- Remove Package "CSS"
- Copy personal preferences file ([Preferences.sublime-settings](/Preferences.sublime-settings))
