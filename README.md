# Guest OS
List for software/dependencies for any guest OS when you want to start developing.. As example for companies..


<br><br>

# Cross Platform
- KeePassXC - Cross-Platform Password Manager (https://keepassxc.org/download/)
- Gitlab Docker (https://hub.docker.com/r/gitlab/gitlab-ce)


<br><br>

# Windows
- Resize Taskbar (https://www.youtube.com/watch?v=ZdXxNOdq4W0)
- Zoom IT (https://docs.microsoft.com/en-us/sysinternals/downloads/zoomit)
- Live Wallpaper (https://rocksdanister.github.io/lively/)
- Confluence Server (https://www.atlassian.com/de/software/confluence/download)

## Guides
- How to create bootable DVD with Windows 10 only (https://www.youtube.com/watch?v=NkySPUcwNhw)

## Errors/Bugs
- DVD Drive not working in Windows 10 [3 SIMPLE METHODS] (https://www.youtube.com/watch?v=VbvSwsIlvxc)









<br><br>

# Linux
- Confluence Server (https://www.atlassian.com/de/software/confluence/download)
- Yakuake Dropdown Terminal (https://apps.kde.org/en/yakuake)
- Clam AV (https://www.clamav.net/downloads)
```bash
# scan full system
sudo clamscan -r /
```

<br><br>
- Kolourpaint
```bash
sudo snap install kolourpaint
```


<br><br>
- Printer drivers
```bash
# xsane is for scanning
# printer-driver-all install all printer drivers
sudo apt install printer-driver-all xsane
```

<br><br>

## ZSH

```bash
sudo apt install zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-history-substring-search.git ~/.oh-my-zsh/custom/plugins/zsh-history-substring-search
git clone https://github.com/powerline/fonts.git
cd fonts
./install.sh
```

<br>~/.zshrc
```
plugins=(
  git 
  zsh-syntax-highlighting
  zsh-history-substring-search
  common-aliases
  history
  extract
  dirhistory
  sudo
  wd  
  fedora
  dnf 
  z
)
ZSH_THEME="agnoster"
```

<br>~/.bashrc
```
# disable user in terminal
PS1="\w \$ "
```









<br><br>

## Fedora
- ZSH (https://kifarunix.com/install-and-setup-zsh-and-oh-my-zsh-on-fedora-32/)

```bash
sudo dnf install make automake gcc gcc-c++ kernel-devel zsh
```

## Guides
- How to run GitLab in a docker container (https://www.youtube.com/watch?v=sLnbWGN77Uc)






<br><br>

## Ubuntu/Kubuntu
- Live Wallpaper (https://github.com/cheesecakeufo/komorebi)
- GUFW (http://gufw.org/)

<br><br>

#### dependencies
```bash
sudo apt update
sudo apt install snapd
sudo snap install snap-store
```

<br><br>

#### Pulse Effects
```bash
sudo apt install pulseffects
```



#### Security
```bash
sudo apt purge avahi-daemon

sudo ufw enable
sudo ufw default deny incoming
sudo ufw default deny forward
sudo ufw default deny outgoing

# find your internet device
ifconfig -a
# allow internet for your device
sudo ufw allow out on <interface> to 1.1.1.1 proto udp port 53 comment 'allow DNS on <interface>'
sudo ufw allow out on <interface> to any proto tcp port 80 comment 'allow HTTP on <interface>'
sudo ufw allow out on <interface> to any proto tcp port 443 comment 'allow HTTPS on <interface>'

# Nordvpn DNS
sudo ufw allow out on nordlynx to 103.86.96.100 proto udp port 53 comment 'allow DNS on <interface>'
sudo ufw allow out on nordlynx to 103.86.99.100 proto udp port 53 comment 'allow DNS on <interface>'
sudo ufw allow out on <ethernetnamehere> to 103.86.99.100 proto udp port 53 comment 'allow DNS on <interface>'
sudo ufw allow out on <ethernetnamehere> to 103.86.96.100 proto udp port 53 comment 'allow DNS on <interface>'

# show rules
sudo ufw status numbered
```

<br><br>

#### Sandbox
- https://null-byte.wonderhowto.com/how-to/locking-down-linux-using-ubuntu-as-your-primary-os-part-3-application-hardening-sandboxing-0185710/
- https://www.youtube.com/watch?v=PQo9PEdVuIw
- https://github.com/CyberT33N/firejail-cheat-sheet
```bash
sudo apt-get install apparmor-profiles apparmor-utils
sudo aa-enforce /etc/apparmor.d/*
sudo apt install firejail
```

#### firejail all paramater
https://firejail.wordpress.com/features-3/man-firejail/



<br><br>


#### KDE
```bash
sudo apt install kde-full

# later choose SDDM display manager
```

<br><br>

#### disable Baloo
```bash
# You may have to create a autostart script for this because after restart it will start again
balooctrl disable
```

<br><br>

#### Change Scale
```bash
gsettings set org.gnome.desktop.interface text-scaling-factor 1.2
```

#### Execute .sh files on double click
- https://askubuntu.com/questions/138908/how-to-execute-a-script-just-by-double-clicking-like-exe-files-in-windows/1255819#1255819

#### Increase Scroll Speed
- https://dev.to/bbavouzet/ubuntu-20-04-mouse-scroll-wheel-speed-536o
```bash
## Install imwheel
sudo apt install imwheel

## create bash script and save anywhere
#!/bin/bash
# Version 0.1 Tuesday, 07 May 2013
# Comments and complaints http://www.nicknorton.net
# GUI for mouse wheel speed using imwheel in Gnome
# imwheel needs to be installed for this script to work
# sudo apt-get install imwheel
# Pretty much hard wired to only use a mouse with
# left, right and wheel in the middle.
# If you have a mouse with complications or special needs,
# use the command xev to find what your wheel does.
#
### see if imwheel config exists, if not create it ###
if [ ! -f ~/.imwheelrc ]
then
cat >~/.imwheelrc<<EOF
".*"
None,      Up,   Button4, 1
None,      Down, Button5, 1
Control_L, Up,   Control_L|Button4
Control_L, Down, Control_L|Button5
Shift_L,   Up,   Shift_L|Button4
Shift_L,   Down, Shift_L|Button5
EOF
fi
##########################################################
CURRENT_VALUE=$(awk -F 'Button4,' '{print $2}' ~/.imwheelrc)
NEW_VALUE=$(zenity --scale --window-icon=info --ok-label=Apply --title="Wheelies" --text "Mouse wheel speed:" --min-value=1 --max-value=100 --value="$CURRENT_VALUE" --step 1)
if [ "$NEW_VALUE" == "" ];
then exit 0
fi
sed -i "s/\($TARGET_KEY *Button4, *\).*/\1$NEW_VALUE/" ~/.imwheelrc # find the string Button4, and write new value.
sed -i "s/\($TARGET_KEY *Button5, *\).*/\1$NEW_VALUE/" ~/.imwheelrc # find the string Button5, and write new value.
cat ~/.imwheelrc
imwheel -kill

# Then set up the .sh file to executable with:
chmod +x mousewheel.sh

# And then run script with:
./mousewheel.sh
```























<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>

# Docker

## Install

#### Ubuntu
```bash
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt update
sudo apt install docker-ce
```










<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>

# Git

## Enable some colorization of Git output.
```bash
git config --global color.ui auto
```


## SSH
- https://github.com/CyberT33N/git-cheat-sheet/blob/main/README.md#ssh



## GUI
GitKraken (PREMIUM - Cross Platform): https://www.gitkraken.com/download
<br>Sourcetree (FREE - Windows & MAC): https://www.sourcetreeapp.com/













<br><br>
 _____________________________________________________
 _____________________________________________________

<br><br>

# Fonts
- https://github.com/tonsky/FiraCode
- https://pcaro.es/d/full-hermit-2.0.tar.gz














<br><br>
 _____________________________________________________
 _____________________________________________________

<br><br>


# Node.js 

## Windows
https://nodejs.org/dist/v15.0.1/node-v15.0.1-x64.msi

<br><br><br><br>

## MAC
https://nodejs.org/dist/v15.0.1/node-v15.0.1.pkg

<br><br><br><br>

## Linux

#### NVM (https://github.com/nvm-sh/nvm)
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash

# if nvm is not working try this
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```

<br><br>

#### Debian (Ubuntu, Mint, ..)
```bash
cd "$(dirname "$0")"
pwd
printf "\nWe will display now the current directory used:"
echo "$(dirname "$0")"
printf "\n\nWe will deinstall now everything with Node.js..\n"
#-------------------------------------------------------------------------------
sudo apt-get remove -y npm
sudo apt-get remove -y nodejs-legacy
sudo apt-get remove -y nodejs
sudo rm /usr/bin/node
sudo rm /usr/local/node
sudo apt -y autoremove
#-------------------------------------------------------------------------------
printf "\n\nWe will download an install now Node.js 15.x\n"
curl -sL https://deb.nodesource.com/setup_15.x | sudo -E bash -
sudo apt-get install -y nodejs
#-------------------------------------------------------------------------------
printf "\n\nWe will display now the current installed version of node:\n"
node -v
printf "\n\nWe will display now the current installed version of npm:\n"
npm -v
#-------------------------------------------------------------------------------
printf "\nWe finished the .sh file :) - Created by Dennis Demand( https://github.com/CyberT33N )\n"
```

#### RPM (Fedora, CentOS, ..)
```bash
cd "$(dirname "$0")"
pwd
printf "\nWe will display now the current directory used:"
echo "$(dirname "$0")"
printf "\n\nWe will deinstall now everything with Node.js..\n"
#-------------------------------------------------------------------------------
sudo yum -y remove nodejs
#-------------------------------------------------------------------------------
printf "\n\nWe will download an install now Node.js 15.x\n"
curl --silent --location https://rpm.nodesource.com/setup_15.x | sudo bash -
sudo yum -y install nodejs
#-------------------------------------------------------------------------------
printf "\n\nWe will display nowhttps://www.jetbrains.com/webstorm/guide/tips/soft-wraps/ the current installed version of node:\n"
node -v
printf "\n\nWe will display now the current installed version of npm:\n"
npm -v
#-------------------------------------------------------------------------------
printf "\nWe finished the .sh file :) - Created by Dennis Demand( https://github.com/CyberT33N )\n"
```

<br />
<br />

## Dependencies
```bash
sudo apt install jupyter-core jupyter-notebook jupyter-client jupyter-console
npm i -g typescript nodemon ijavascript node-gyp
ijavascript
```


<br><br>
 _____________________________________________________
 _____________________________________________________

<br><br>

# Webstorm (https://www.jetbrains.com/de-de/webstorm/)

## Plugins
- Atom Material Icons
- Tabnine
- CodeGlance (Minimap)
- Pokemon Progress
- Activate-power-mode (https://plugins.jetbrains.com/plugin/14000-activate-power-mode-x)
- Power Mode II
- Rainbow Brackets
- Sexy Editor (https://plugins.jetbrains.com/plugin/1833-sexy-editor)
- Anime Memes (https://plugins.jetbrains.com/plugin/15865-anime-memes)
- Rainbow Fart (https://plugins.jetbrains.com/plugin/14543-rainbow-fart)
- Fancy music (https://plugins.jetbrains.com/plugin/13231-fancy-music)
- Key Promoter X (https://plugins.jetbrains.com/plugin/9792-key-promoter-x)

<br><br>

## Enable Zoom with CTRL + Mouse Wheel
- In the Settings/Preferences dialog Ctrl+Alt+S, select Editor | General. Make sure that the setting Change font size (Zoom) with Ctrl+MouseWheel is enabled.

<br><br>

## Add Unit Tests Sidebar
- Edit Configuration (top right)
<br> -> Choose Mocha package
<br> -> User Interface: **bdd**
<br> -> Extra Mocha options: **--recursive --exit --timeout 30000**
<br> -> File Patterns: **./test/*.test.js**






<br><br> <br><br>

## Enable auto render of JSDoc
- open the Settings/Preferences dialog Ctrl+Alt+S, go to Editor | General | Appearance, and select the Render documentation comments checkbox.










<br><br><br><br>

## Fonts

<br><br>

#### Change Fonts
- File > Settings > Editor > Font

<br><br>

#### Bold Fonts
- File > Settings > Color Scheme > General > Text > Default Text > Bold
- You can to File > Settings > Color Scheme > Javascript to change as example function params to bold too




<br><br>

## disable auto indent
- In  File | Settings | Editor | General | Smart Keys you need to disable Smart indent (this should help for cases when "CLion still sometimes inserts tabs when i dont press TAB key") and set Reformat on paste to None (this should help for cases when "CLion deletes tabs from lines that i paste"):


<br><br>


## Create Desktop Shortcut
- Tools > Create Desktop Entry

<br><br>


## Import Color Scheme
- File > Settings > Editor > Color Scheme > Settings Wheel Icon > Import Scheme
- You can import .xml or .icls
- https://www.jetbrains.com/help/webstorm/settings-colors-and-fonts.html

<br><br>

## Sublime Syntax Color Scheme
- https://gist.github.com/CyberT33N/a3905f0b9da8cebb42d03998d79b6a5f **FINAL almost like atom**
- https://plugins.jetbrains.com/plugin/12773-onedarkmonokai
- https://github.com/darekkay/config-files/blob/master/intellij-idea/config/colors/dk-monokai.icls


<br><br>
<br><br>

## Soft Wraps
- Preferences/Settings | Editor | General > Soft-wrap files (https://www.jetbrains.com/webstorm/guide/tips/soft-wraps/)


<br><br>

## Eslint
- File > Settings > Search: eslint

<br><br>

## Vertical Line Indentation
- Go to Settings/Editor/General/Appearance and select **Show indent guides** to enable this feature in IntelliJ. (https://i.stack.imgur.com/NsoJV.png)

<br><br>
 _____________________________________________________
 _____________________________________________________

<br><br>

# Atom (https://atom.io/)

<br><br>

## Enable Vertical Lines
Settings > Editor > Show Indent Guide

## Enable Line Wrap
File > Config
<br><br>
Add 'softWrap':true to the 'editor' section like this:
```cson
'editor':
  'softWrap': true
```

<br>
<br>


## Packages
```bash
apm install highlight-selected atom-beautify pigments emmet minimap minimap-cursorline minimap-find-and-replace minimap-pigments atom-increment neon-selection iv-terminal typescript teletype atom-scale-factor atom-markdown-auto-preview logo-file-icons atom-live-server script linter-htmllint linter-csslint linter-eslint hydrogen
```
- https://atom.io/packages/highlight-selected (https://youtu.be/aiXNKHKWlmY?t=1549)
- https://atom.io/packages/atom-beautify (https://youtu.be/aiXNKHKWlmY?t=1395)
- https://atom.io/packages/pigments (https://youtu.be/aiXNKHKWlmY?t=993)
- https://atom.io/packages/emmet (https://youtu.be/aiXNKHKWlmY?t=204)
- https://atom.io/packages/minimap
- https://atom.io/packages/minimap-cursorline
- https://atom.io/packages/minimap-find-and-replace
- https://atom.io/packages/minimap-pigments
- https://atom.io/packages/atom-increment
- https://atom.io/packages/neon-selection
- https://atom.io/packages/iv-terminal
- https://atom.io/packages/typescript
- https://atom.io/packages/teletype
- https://atom.io/packages/atom-scale-factor
- https://atom.io/packages/atom-markdown-auto-preview
- https://atom.io/packages/logo-file-icons
- https://atom.io/packages/atom-live-server (https://www.youtube.com/watch?v=0Xy3yDDY4IE)
- https://atom.io/packages/script
- https://atom.io/packages/linter-htmllint
- https://atom.io/packages/linter-csslint
- https://atom.io/packages/linter-eslint (https://www.youtube.com/watch?v=dG9EEkSCbWM)
- https://atom.io/packages/hydrogen (https://nteract.gitbooks.io/hydrogen/content | https://www.youtube.com/watch?v=VcDbxEV-OI0)
<br> If you got missing lib folder error try: apm install hydrogen@2.9.0



<br><br>



## Linter
- Disable Linter (https://atom.io/packages/linter) if installed and use Diagnostics of atom-ide-ui instead (Packages > atom-ide-ui > Settings > Enabled Features > Diagnostics).

#### htmllint
```bash
npm install htmllint --save-dev
```
<br>

#### .htmllintrc
```json
{
  "indent-width": 2
}
```


<br><br>

#### eslint
```bash
npm install eslint --save-dev
```

#### .eslintrc.yml
```yml
env:
  browser: true
  es2021: true
  node: true
extends:
  - google
parserOptions:
  ecmaVersion: 12
  sourceType: module
rules:
  arrow-parens: off
  brace-style: off
```


<br><br>



## Syntax
atom-sublime-monokai-syntax



<br />
<br />

## styles.less (File > Stylesheet)
```css
atom-text-editor {
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  font-family: "Hermit"; /* change font here.. */
  font-weight: 500;
  line-height: 1.7;
  background: #191919;
}

atom-text-editor.editor {
  .syntax--storage.syntax--type.syntax--function.syntax--arrow,
  .syntax--keyword.syntax--operator:not(.accessor),
  .syntax--punctuation.syntax--definition {
    font-family: "Fira Code";
  }

  .syntax--string.syntax--quoted,
  .syntax--string.syntax--regexp {
    -webkit-font-feature-settings: "liga" off, "calt" off;
  }
}


atom-text-editor .cursor {
   border-color: white;
   border-width: .2vmax;
}
```

