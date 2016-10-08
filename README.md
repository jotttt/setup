# setup
Links and preferences for quick setup of personal development environment

## Heavily borrowed from following pages
- Windows - https://scotch.io/tutorials/get-a-functional-and-sleek-console-in-windows
- https://github.com/mdo/config

## Setup Windows
- Install [Git](https://git-scm.com/download/win)
- Install [ConEmu](https://conemu.github.io/)
- Choose `{Bash::Git bash}` as startup task on inital launch config
- Open Settings and Import [`ConEmu.xml`](ConEmu.xml)
- Copy [`.bash_profile`](.bash_profile) to User home directory (`%HOMEPATH`)
- If needed, add a line in bash profile to fast navigate to default dev directory `cd f:/dev`
- Reload bash profile `source ~/.bash_profile`


## Dev dependencies
- Grunt `npm install -g grunt-cli`


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
