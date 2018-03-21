# setup
Links and preferences for quick setup of personal development environment

## Windows
- copy ssh keys from Dropbox to -> users/[username]/.ssh/
- Install [WinSCP](https://winscp.net/eng/download.php) and go to tools -> import settings file from Dropbox
- Install [Node.js](https://nodejs.org/en/) 
- Install [Git](https://git-scm.com/download/win)
- Install [ConEmu](https://conemu.github.io/)
- Choose `{Bash::Git bash}` as startup task on inital launch config
  - If there is error, point startup task to -> program files/git/bin/sh.exe
- Open Settings and Import [`ConEmu.xml`](ConEmu.xml)

## React.js
### [create-react-app](https://github.com/facebook/create-react-app) 
- `npm install -g create-react-app`
- to create a new React.js project run `create-react-app my-app`

### Atom 
- Install [Atom](https://atom.io/)
- install 

## Dev dependencies
- Gulp `npm install -g gulp`

## Brackets 
- Install [Brackets](http://brackets.io/)
- Install Brackets extensions:
  - Extensions Bulk Installer (use the config file in Dropbox)
- Copy brackets.json file from Dropbox to \Users\[username]\AppData\Roaming\Brackets
- Add EditorConfig file to webdev root

## TTU
- Go to -> https://wiki.ttu.ee/it/et/doc/vpn and install the vpn client
- Start vpn and go to https://itwiki.intra.ttu.ee/ Search git to get repo addresses 

## Inkscape (with dark theme)
- Install inkscape 0.91 -> https://inkscape.org/en/release/0.91/ 
- Copy files from dropbox/webdev/setup/inkscape/dark theme files to C:\Program Files\Inkscape\
- Copy default template from dropbox/webdev/setup/inkscape to C:\Program Files\Inkscape\share\templates OR C:\Users\[username]\AppData\Roaming\inkscape\templates
- Start or re-start Inkscape

## Gimp (with photoshop-like dark theme and tweaks)
- Install dark version Gimp 2.8.14 [[Link](http://www.partha.com/)]
- copy plug-ins (Content Aware Fill and Layer via copy extensions) folder content to users/[username]/.gimp-2.8/plug-ins
- Copy themes folder content to users/[username]/.gimp-2.8/themes
  - open the program, select Windows -> Single-Window Mode...
  - select the theme, from Edit -> Preferences -> Theme
  - drag the tools Panel to the right and shrink the left tools panel, so it only has two rows
- Copy menurc (photoshop-like shortcuts) file to users/[username]/.gimp-2.8/
- Copy gimprc (Turn on the "Snap to Canvas Edge" option by default) file to users/[username]/.gimp-2.8/
- Disable the layer boundary
  - go to Edit -> Preferences -> Image Windows - Appearance and uncheck the "Show Layer Boundary" in both Normal and full-screen Mode.
- Change how the Move Tool works
  - with the Move Tool selected, we choose the "Move the active layer" option...
  - ...and then we go to Edit -> Preferences -> Tools Options -> Save Tool Options Now.
- Copy gimp-splash.png (photoshop cs6 inspired) from splash folder to C:\Program Files\Gimp-2.8\share\gimp\2.0\images

## Sumatra PDF 
- don't install Adobe Reader or Foxit PDF
