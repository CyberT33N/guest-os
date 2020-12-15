# Guest OS
List for software/dependencies for any guest OS when you want to start developing.. As example for companies..



# Windows
- Resize Taskbar (https://www.youtube.com/watch?v=ZdXxNOdq4W0)
- Zoom IT (https://docs.microsoft.com/en-us/sysinternals/downloads/zoomit)
- Live Wallpaper (https://rocksdanister.github.io/lively/)


<br><br>

# Linux

<br>

## Ubuntu
- Live Wallpaper (https://github.com/cheesecakeufo/komorebi)

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


<br>
<br>



 _____________________________________________________
 _____________________________________________________



<br>

<br>
<br>

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

<br>
<br>



 _____________________________________________________
 _____________________________________________________



<br>
<br>

# Fonts
- https://github.com/tonsky/FiraCode
- https://pcaro.es/d/full-hermit-2.0.tar.gz




 _____________________________________________________
 _____________________________________________________


<br />
<br />


# Node.js 

## Windows
https://nodejs.org/dist/v15.0.1/node-v15.0.1-x64.msi

## MAC
https://nodejs.org/dist/v15.0.1/node-v15.0.1.pkg

## Linux

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
printf "\n\nWe will display now the current installed version of node:\n"
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
npm i -g typescript nodemon eslint ijavascript
ijavascript
```


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
apm install highlight-selected atom-beautify pigments emmet minimap minimap-cursorline minimap-find-and-replace minimap-pigments atom-increment neon-selection iv-terminal typescript teletype atom-scale-factor atom-markdown-auto-preview logo-file-icons atom-live-server script linter-eslint hydrogen
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
- https://atom.io/packages/linter-eslint (https://www.youtube.com/watch?v=dG9EEkSCbWM)
- https://atom.io/packages/hydrogen (https://nteract.gitbooks.io/hydrogen/content | https://www.youtube.com/watch?v=VcDbxEV-OI0)
<br> If you got missing lib folder error try: apm install hydrogen@2.9.0



<br />
<br />

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

