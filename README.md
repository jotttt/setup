# setup
Links and preferences for quick setup of personal development environment

## Heavily borrowed from following pages
- Windows - https://scotch.io/tutorials/get-a-functional-and-sleek-console-in-windows
- https://github.com/mdo/config

## Setup Windows
- copy ssh keys from Dropbox to -> users/[username]/.ssh/
- Install [WinSCP](https://winscp.net/eng/download.php) and go to tools -> import settings file from Dropbox
- Install [Node.js](https://nodejs.org/en/) 
- Install [Git](https://git-scm.com/download/win)
- Install [ConEmu](https://conemu.github.io/)
- Choose `{Bash::Git bash}` as startup task on inital launch config
  - If there is error, point startup task to -> program files/git/bin/sh.exe
- Open Settings and Import [`ConEmu.xml`](ConEmu.xml)

## Dev dependencies
- Gulp `npm install -g gulp`

## Brackets 
- Install Brackets [[Link](http://brackets.io/)]
- Install Brackets extensions:
  - Extensions Bulk Installer (use the config file in Dropbox)
- Copy brackets.json file from Dropbox to \Users\[username]\AppData\Roaming\Brackets
- Add EditorConfig file to webdev root

## TTU
- Go to -> https://wiki.ttu.ee/it/et/doc/vpn and install the vpn client
- Start vpn and go to https://itwiki.intra.ttu.ee/ to get repo addresses 

## Inkscape 
- 

## Gimp (with photoshop like tweaks)
- Install Gimp 2.8.14 [[Link](http://www.partha.com/)]
- Install Gimp extensions:
  - Photoshop themes [[Link](http://migf1.deviantart.com/art/Clearlooks-Flat-Icons-Gimp-2-8-Themes-v-1-0-1-484289796)]
  - Photoshop like shortcuts [[Link](http://epierce.freeshell.org/gimp/gimp_ps.php)]
  - Content Aware Fill [[Link](http://epierce.freeshell.org/gimp/gimp_ps.php)]
    - download the zip folder
    - extract the content of the PluginScripts folder to users/[username]/.gimp-2.8/plug-ins
  - Layer via copy [[Link](http://gimper.net/resources/layer-via-copy-cut.417/)]
    - copy the layer-via-copy-cut.py file to .gimp-2.8/plug-ins/
- Turn on the "Snap to Canvas Edge" option by default
  - in users/[username]/.gimp-2.8 open gimprc with notepad and paste these lines at the very end:
    (default-snap-to-canvas yes)
    (default-snap-to-grid yes)
- Disable the layer boundary
  - go to Edit -> Preferences -> Image Windows - Appearance and uncheck the "Show Layer Boundary" in both Normal and full-screen Mode.
- Change how the Move Tool works
  - with the Move Tool selected, we choose the "Move the active layer" option...
  - ...and then we go to Edit -> Preferences -> Tools Options -> Save Tool Options Now.
- Change splashscreen
  - name the image gimp-splash.png
  - replace the image in C:\Program Files\Gimp-2.8\share\gimp\2.0\images
