# setup
Links and preferences for quick setup of personal development environment

## 1. [Chocolatey](https://chocolatey.org/) - package manager for Windows

**Install Chocolatey**
- Run as admin PowerShell.exe
- Then run `Get-ExecutionPolicy`. If it returns `Restricted`, then run `Set-ExecutionPolicy AllSigned` or `Set-ExecutionPolicy Bypass -Scope Process`.
- Then run `Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object                                              System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`

**Install packages**
- Install [WinSCP](https://winscp.net) `choco install winscp`
  - go to tools -> import settings file from Dropbox
- Install [Node.js](https://nodejs.org/en/) `choco install nodejs`
- Install [Git](https://git-scm.com/) `choco install git`
- Install [ConEmu](https://conemu.github.io/) `choco install conemu`
  - Choose `{Bash::Git bash}` as startup task on inital launch config
  - If there is error, point startup task to -> program files/git/bin/sh.exe
  - Open Settings and Import [`ConEmu.xml`](ConEmu.xml)
- install [VS Code](https://code.visualstudio.com/) `choco install visualstudiocode`
>
>*combined command:* `choco install winscp nodejs git conemu visualstudiocode`
>

## 2. [VS Code](https://code.visualstudio.com/) - IDE

**sync with GitHub**


## 3. [React.js](https://reactjs.org/) - A JavaScript library for building user interfaces

**[create-react-app](https://github.com/facebook/create-react-app)** - Create React app with no build configuration
- to install `npm install -g create-react-app`
- to create a new React.js project `create-react-app my-app-name`
- move to folder `cd my-app-name`
- start dev server `npm start`

**[ESLint](https://eslint.org/)** - React.js specific linting config
- install packages `npm install --save-dev eslint babel-eslint eslint-config-react eslint-plugin-react eslint-plugin-react-native`
- add [.eslintrc.json](https://github.com/jotttt/setup/blob/master/ESLint/.eslintrc.json) to project root  

**[Sass](https://sass-lang.com/)** - Css pre-processor for create-react-app
- to install `npm install --save node-sass-chokidar npm-run-all`
- Then in package.json, add the following lines to scripts: 
```
      "scripts": {
+    "build-css": "node-sass-chokidar src/ -o src/",
+    "watch-css": "npm run build-css && node-sass-chokidar src/ -o src/ --watch --recursive",
-    "start": "react-scripts start",
-    "build": "react-scripts build",
+    "start-js": "react-scripts start",
+    "start": "npm-run-all -p watch-css start-js",
+    "build-js": "react-scripts build",
+    "build": "npm-run-all build-css build-js",
     "test": "react-scripts test --env=jsdom",
     "eject": "react-scripts eject"
   }
```
- Now running npm start and npm run build also builds Sass files, finding every Sass file in src subdirectories and creating a corresponding CSS file next to it.

**[Bootstrap 4](https://getbootstrap.com/)** - Front-end component library
- to install `npm install --save bootstrap`
- add import line to index.js:
```
import 'bootstrap/dist/css/bootstrap.min.css';
```

**[ReactStrap](https://reactstrap.github.io/)** - Bootstrap integration for React
- to install `npm install --save reactstrap@next`
- Import required reactstrap components within src/App.js file or your custom component files ie:
```
import { Button } from 'reactstrap';
```
- check how to use different components from here: https://reactstrap.github.io/components/alerts/ 

**[Font Awesome](https://fontawesome.com/)** - Icon library
- to install `npm install --save font-awesome`
- add import line to index.js:
```  
import 'font-awesome/css/font-awesome.min.css';
```

**Custom fonts**
- to install ie. Open Sans font `npm install --save typeface-open-sans`
- add import line to index.js:
```  
import 'typeface-open-sans';
```
## Other tools

### Brackets
- Install [Brackets](http://brackets.io/)
- Install Brackets extensions:
  - Extensions Bulk Installer (use the config file in Dropbox)
- Copy brackets.json file from Dropbox to \Users\[username]\AppData\Roaming\Brackets
- Add EditorConfig file to webdev root

### TTU
- Go to -> https://wiki.ttu.ee/it/et/doc/vpn and install the vpn client
- Start vpn and go to https://itwiki.intra.ttu.ee/ Search git to get repo addresses
- copy ssh keys from Dropbox to -> users/[username]/.ssh/

### Inkscape (with dark theme)
- Install inkscape 0.91 -> https://inkscape.org/en/release/0.91/
- Copy files from dropbox/webdev/setup/inkscape/dark theme files to C:\Program Files\Inkscape\
- Copy default template from dropbox/webdev/setup/inkscape to C:\Program Files\Inkscape\share\templates OR C:\Users\[username]\AppData\Roaming\inkscape\templates
- Start or re-start Inkscape

### Gimp (with photoshop-like dark theme and tweaks)
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

### [Pencil](http://pencil.evolus.vn/) - Wireframing tool
- 

### Sumatra PDF
- don't install Adobe Reader or Foxit PDF
