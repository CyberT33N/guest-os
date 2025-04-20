# Guest OS
List for software/dependencies for any guest OS when you want to start developing.. As example for companies..












<br><br>

# Cross Platform
- KeePassXC - Cross-Platform Password Manager (https://keepassxc.org/download/)
- Gitlab Docker (https://hub.docker.com/r/gitlab/gitlab-ce)


## Firefoxc

### Extensions
- https://addons.mozilla.org/en-US/firefox/addon/hls-downloader/
  - https://github.com/puemos/hls-downloader 


<br><br>

## Chromium

#### Extension
- Script Safe (https://chrome.google.com/webstore/detail/scriptsafe/oiigbmnaadbkfbmpbfijlflahbdbdgdf)
- Webrtc Anti Leak Prevent (https://chrome.google.com/webstore/detail/webrtc-leak-prevent/eiadekoaikejlgdbkbdfeijglgfdalml)
- Nimbus (https://chrome.google.com/webstore/detail/nimbus-screenshot-screen/bpconcjcammlapcogcnnelfmaeghhagj/related)











<br><br>
<br><br>
___________________________________________
<br><br>
<br><br>

# Windows
- Resize Taskbar (https://www.youtube.com/watch?v=ZdXxNOdq4W0)
- Zoom IT (https://docs.microsoft.com/en-us/sysinternals/downloads/zoomit)
- Live Wallpaper (https://rocksdanister.github.io/lively/)
- Confluence Server (https://www.atlassian.com/de/software/confluence/download)

<br><br>

## Guides
- How to create bootable DVD with Windows 10 only (https://www.youtube.com/watch?v=NkySPUcwNhw)

<br><br>

## Errors/Bugs
- DVD Drive not working in Windows 10 [3 SIMPLE METHODS] (https://www.youtube.com/watch?v=VbvSwsIlvxc)

<br><br>

## Package Manager
- https://github.com/CyberT33N/chocolatey-cheat-sheet


<br><br>

## Utils

### Anti afk

<details><summary>Click to expand..</summary>

Method #1 - Autohot key
```
; Setzt einen Timer, der die Funktion MoveMouse alle 1000 Millisekunden (1 Sekunde) aufruft.
SetTimer(MoveMouse, 1000)

; Diese Funktion wird regelmäßig durch den Timer aufgerufen.
MoveMouse() {
    ; Prüft, ob der Computer für mehr als 150.000 Millisekunden (150 Sekunden = 2,5 Minuten) inaktiv war.
    if (A_TimeIdle > 25000) {
        ; Bewegt die Maus um 20 Pixel nach rechts und 30 Pixel nach unten mit einer Geschwindigkeit von 35.
        ; Das "R" bedeutet, dass die Bewegung relativ zur aktuellen Mausposition erfolgt.
        MouseMove(20, 30, 35, "R")
        
        ; Bewegt die Maus zurück um 20 Pixel nach links und 30 Pixel nach oben mit derselben Geschwindigkeit.
        MouseMove(-20, -30, 35, "R")
    }
}

; Beendet das Skript, wenn die Escape-Taste gedrückt wird.
Esc::ExitApp

```

Es gibt mehrere Wege, dein AutoHotkey-Skript beim Start von Windows automatisch auszuführen:  

### **Methode 1: Skript in den Autostart-Ordner legen** (einfachste Methode)  
1. **Drücke** `Win + R`, gib ein:  
   ```
   shell:startup
   ```
   **und drücke Enter**. Das öffnet den Autostart-Ordner.  
2. **Ziehe** dein `.ahk`-Skript oder eine Verknüpfung davon in diesen Ordner.  
3. Beim nächsten Start wird es automatisch ausgeführt.  

---

### **Methode 2: Geplante Aufgabe erstellen** (falls Adminrechte nötig sind)  
Falls dein Skript Adminrechte braucht oder du es mit Verzögerung starten willst:  
1. **Drücke** `Win + S`, suche nach „Aufgabenplanung“ und öffne sie.  
2. Klicke rechts auf „Einfache Aufgabe erstellen…“.  
3. Gib einen Namen (z. B. „AutoHotkey Startup“) und klicke „Weiter“.  
4. Wähle **„Beim Start des Computers“** und klicke „Weiter“.  
5. Wähle **„Programm starten“**, dann „Weiter“.  
6. Klicke auf „Durchsuchen“ und wähle dein `.ahk`-Skript aus.  
7. Setze ein Häkchen bei **„Mit höchsten Privilegien ausführen“** (falls Adminrechte nötig).  
8. Klicke auf „Fertig stellen“.  

Damit läuft das Skript jedes Mal beim Hochfahren. 🚀


</details>


























<br><br>
<br><br>
___________________________________________
<br><br>
<br><br>

# Linux
- Confluence Server (https://www.atlassian.com/de/software/confluence/download)

- Yakuake Dropdown Terminal (https://apps.kde.org/en/yakuake)
  - Try first to install it via apps.kde link because there are sometimes problems with the snap version and it wont start
```shell
sudo snap install yakuake --candidate
```

- Clam AV (https://www.clamav.net/downloads)
```bash
# scan full system
sudo clamscan -r /
```


<br><br>
- Postman
```bash
sudo snap install postman
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
- Change at the top ZSH_THEME="agnoster"
- Add this to the bottom:
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
  dnf 
  z
)
```

<br>~/.bashrc
```
# disable user in terminal
PS1="\w \$ "
```









<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>

# jdownloader
https://jdownloader.org/download/index

jdownloader needs java
```shell
sudo apt install default-jdk
```





<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>

# yt-dlp (recommended)
```shell
sudo curl -L https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -o /usr/local/bin/yt-dlp
sudo chmod a+rx /usr/local/bin/yt-dlp

# dl video
yt-dlp "https://www.youtube.com/watch?v=Mjq7kbMM0Bg"

# dl audio
yt-dlp -x --audio-format mp3 "https://www.youtube.com/watch?v=Mjq7kbMM0Bg"
```

<br><br>
<br><br>


# youtube-dl
- If encountered 403 forbidden problems here and used instead yt-dlp
```shell
git clone https://github.com/ytdl-org/youtube-dl.git youtube-dl
cd youtube-dl/
make youtube-dl
sudo cp youtube-dl /usr/local/bin/

# If you get error /usr/bin/env: ‘python’: No such file or directory
# Then install python. If you have python3 then create symlink
sudo ln -s /usr/bin/python3 /usr/bin/python
```
- Usage:
  ```
  youtube-dl https://www.youtube.com/watch?v=Mjq7kbMM0Bg
  ```

- If you get 403 forbidden error try:
```


sudo apt install python3.12-venv

python3 -m venv YOUTUBEDL
source YOUTUBEDL/bin/activate

pip install youtube_dl

python3 -m youtube_dl --user-agent "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/127.0.6533.103 Mobile Safari/537.36" "https://www.youtube.com/watch?v=Mjq7kbMM0Bg" 

deactivate
```



<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>


# OpenRGB
- https://gitlab.com/CalcProgrammer1/OpenRGB#smbus-access

Install this if not all of devices are detected
```shell
sudo apt install i2c-tools
sudo modprobe i2c-dev
sudo groupadd --system i2c
sudo usermod $USER -aG i2c
sudo touch /etc/modules-load.d/i2c.conf && sudo sh -c 'echo "i2c-dev" >> /etc/modules-load.d/i2c.conf'
sudo modprobe i2c-i801
sudo modprobe i2c-nct6775
```

<br><br>


## Plugins
- https://openrgb.org/plugins.html
- https://openrgb.org/releases/plugins/effects/release_0.9/OpenRGBEffectsPlugin_0.9_Bookworm_64_f1411e1.so

<br><br>


### Effects
- make sure to enable effect on the elft side after you add it

<br><br>

#### Good effects
- Advanced > Sunrise
- Advanced > SwirlCircles
- Advanced > Wavy
- Advanced > ZigZag

- Beam > Rotating Beam

- Rainbow > Custom gradient wave
- Rainbow > double rotating rainbow
- Rainbow > radial rainbow
- Rainbow > rainbow wave
- Rainbow > rrotating rainbow **HOT**

- Simple > Fill
- Simple > Motion point



















<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>



# Corsair
- If you want to use icue link which only exists for windows you must use vmware and then run windows. After you start the vm at the bottom right you can enable your corsair devices to the vm. Make sure that you safe your profiles to the internal storage or otherwhise after you close the vm it will be resettedt


<br><br>
<br><br>


## RAM
- If you want to change the color of your RAM you can use use VMware and change it there with iCUE LINK. You must use OpenRGB on your Linux Host


<br><br>
<br><br>

## iCUE LINK H150i LCD

<br><br>


### GIFS
- https://www.reddit.com/r/LoadingIcons/

- https://packaged-media.redd.it/90lrmrx1eskb1/pb/m2-res_1080p.mp4?m=DASHPlaylist.mpd&v=1&e=1720234800&s=cb3b83f945b23de9bc4c7e41963ed4874433004a#t=0
- https://imgur.com/gallery/desync-mI3M8My
- https://www.reddit.com/r/LoadingIcons/comments/15o7w5w/orbit_curves_a/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button
- https://www.reddit.com/r/LoadingIcons/comments/157l17w/o_010617_by_xponentialdesign/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button
- https://preview.redd.it/5jo8ekjaygdb1.gif?width=1080&format=mp4&s=278a8dced1c652178e9b20a1c858ecd4b3bf27c2




<br><br>
<br><br>

## .cueprofile
- https://help.corsair.com/hc/en-us/articles/9399098258189-iCUE-How-to-Import-and-export-iCUE-profiles

<br><br>

### Themes
- If you want to change the themes than disable internal storage first
- https://www.corsair.com/us/en/explorer/icue/icue-profiles/neon/
- https://www.corsair.com/us/en/explorer/icue/icue-profiles/avengers-endgame/
- https://www.corsair.com/us/en/explorer/icue/icue-profiles/halloween-eyes/
- https://www.corsair.com/us/en/explorer/icue/icue-profiles/valorant/
- https://www.corsair.com/us/en/explorer/icue/icue-profiles/apexlegends/

// Maybe old version and not working
- https://rgbprofiles.com/product-category/free-profiles/














<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>






# VMWare
- https://support.broadcom.com/group/ecx/productfiles?subFamily=VMware%20Workstation%20Pro&displayGroup=VMware%20Workstation%20Pro%2017.0%20for%20Personal%20Use%20(Linux)&release=17.5.2&os=&servicePk=520450&language=EN

- If you can not install vmmon and vmnet download 17.5.1 and then:
```shell
wget https://github.com/mkubecek/vmware-host-modules/archive/workstation-17.5.1.tar.gz
tar -xzf workstation-17.5.1.tar.gz
cd vmware-host-modules-workstation-17.5.1/
tar -cf vmmon.tar vmmon-only
tar -cf vmnet.tar vmnet-only
sudo cp -v vmmon.tar vmnet.tar /usr/lib/vmware/modules/source/
sudo vmware-modconfig --console --install-all
```





















<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>


# starship
- https://github.com/CyberT33N/starship-cheat-sheet
















<br><br>
<br><br>
___________________________________________
<br><br>
<br><br>

# Fonts
- https://vercel.com/font **HOT**
- https://www.nerdfonts.com/font-downloads

- https://github.com/tonsky/FiraCode
- https://pcaro.es/d/full-hermit-2.0.tar.gz





















<br><br>
<br><br>
___________________________________________
<br><br>
<br><br>

# System details in terminal
```
sudo apt install neofetch
```












<br><br>
<br><br>
___________________________________________
<br><br>
<br><br>

# KDE


<br><br>
<br><br>



# 🐬 Dolphin Einstellungen
<br><br>
<br><br>

## Schriftart ändern
- Ändere die Schriftart auf "Carda Dings Da"


<br><br>
<br><br>


# 🎨 Konsole Theme
- [Download Link](https://store.kde.org/p/1329371)
- You can add colorschemes here:
  - ~/.local/share/konsole/ 

## Background
- https://www.freepik.com/free-vector/game-live-stream-interface-elements_29836796.htm#fromView=search&page=1&position=10&uuid=8f26d9b1-ac06-4901-98ba-056287c1d4a1
- https://www.freepik.com/free-vector/gradient-pack-twitch-panels_21077582.htm#fromView=search&page=1&position=33&uuid=8f26d9b1-ac06-4901-98ba-056287c1d4a1
- https://www.freepik.com/free-vector/twitch-stream-panels-collection_9147552.htm#fromView=search&page=1&position=36&uuid=8f26d9b1-ac06-4901-98ba-056287c1d4a1


Choose wallpaper and stretch

Go to apperance > Miscellaneous and set
- line spacing 5px
- margin 60px

Alternative you can set it aswell here:
- ~/.local/share/konsole/yourProfile
```
[Appearance]
ColorScheme=Amethyst
Font=CaskaydiaCove Nerd Font,10,-1,5,50,0,0,0,0,0

[General]
Name=t33n
Parent=FALLBACK/
TerminalColumns=120
TerminalMargin=40
TerminalRows=48

[Scrolling]
HistorySize=100000
```


apperance > cursor
- enable blinking

apperance > color scheme & font
- select font caskaydiacove nerd font


scrolling > scrollback > change to 100000 for icnreased buffer
scrolling > scrollbar position:hidden









<br><br>
<br><br>

<br><br>
<br><br>

# 🛠 Widgets

## 💬 ChatGPT
- [Download Link](https://store.kde.org/p/1977771)

## 🌐 NordVPN
- [Download Link](https://store.kde.org/p/1689651)

## 🎵 Audio Visualizer

### Panon
- [GitHub Repository](https://github.com/rbn42/panon)

```shell
sudo apt-get install qml-module-qt-websockets python3-docopt python3-numpy python3-pyaudio python3-cffi python3-websockets qt5-websockets python3-docopt python3-numpy python3-pyaudio python3-cffi python3-websockets pipewire-pulse pipewire-alsa pipewire-jack pipewire

sudo pip install -U websockets
```

### Installation via KDE Store
1. Öffne den “Add Widgets” Dialog auf deinem Desktop
2. Gehe zu “Get New Widgets” am unteren Rand
3. Klicke auf “Download New Plasma Widgets”
4. Suche nach “panon”
5. Klicke auf “Install”

### Widget Einstellungen
- Füge das Widget hinzu und gehe zu den Einstellungen, dort kannst du neue Effekte herunterladen
- Wähle “advanced circular” und nutze die folgenden Einstellungen:

```
Number of units: 50
Unit fill: 60
Inner radius: 0.4

Enable fit in low and high

Drift factor: 0.1

Divide circle into n arc: 2

p values can be all 1

Enable proportional scaling

Enable update UV every frame
```

### Back-End Tab
- Verwende PortAudio und Frequenzbereich 0 bis 600 Hz

### Farb Tab
- Hue von: 50
- Hue bis: 50
- Sättigung: 100
- Helligkeit: 90

### Widget Bearbeiten
- Rechtsklick auf das Widget und unter "Widget bearbeiten" den Hintergrund deaktivieren

### Effekt "rbn" herunterladen
- Lade den Effekt herunter und platziere ihn über der Taskleiste im Bearbeitungsmodus
- Bei visuellen Effekten > Balkenbreite nutze 5

### Farben Tab
- Hue von: 50
- Hue bis: 50
- Sättigung: 100
- Helligkeit: 90

## ⏰ Clock
- [Download Link](https://store.kde.org/p/1666554)

## 🐾 Animated Pets
- [Download Link](https://store.kde.org/p/1349326)

## ⚽ Bouncing Ball
- [Download Link](https://store.kde.org/p/1172489)
- Einstellungen:
  - Schwerkraft: 1.50
  - Reibung: 0.03
  - Rückprall: 0.8
  - Tick Länge: 20ms

# ⚙️ Einstellungen

## Erscheinungsbild
- Gehe zu Einstellungen > Erscheinungsbild > Desktop Effekte > Neue holen
  - Geometry Change für Plasma 5
  - Fold Popups
  - Lightly Shaders
- Aktiviere alle in den Einstellungen

# 🖥 KWin Scripting
- Du kannst KWin Scripts unter Einstellungen > Fensterverwaltung > KWin Scripts hinzufügen
  - Suche nach:
    - Karousel
    - Windows Gaps
    - No Border Firefox
    - Tiling


## icons
- https://store.kde.org/p/2112373

# splash screen
- https://store.kde.org/p/1871282
- https://store.kde.org/p/1427916

# boot splash screen
- https://store.kde.org/p/1635081

# font
- caskaydiamono nerd font
- for window title hurmit nerd font bold

# cursor
- https://store.kde.org/p/1457141

# GTK3/4 Themes
- https://www.gnome-look.org/p/1214931


# window decoration
- https://store.kde.org/p/1172409
- https://store.kde.org/p/1356759 **hot**




# color scheme
- https://store.kde.org/p/1965725



# color theme

## yaru-colors
- https://snapcraft.io/yaru-colors
```shell
snap install yaru-colors
for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i yaru-colors:gtk-3-themes; done && for i in $(snap connections | grep gtk-common-themes:gtk-2-themes | awk '{print $2}'); do sudo snap connect $i yaru-colors:gtk-2-themes; done && for i in $(snap connections | grep gtk-common-themes:icon-themes | awk '{print $2}'); do sudo snap connect $i yaru-colors:icon-themes; done

# then relogin
```



<br><br>

## Window Effects

<br><br>

### Burn my Windows
- https://github.com/Schneegans/Burn-My-Windows
```shell
wget https://github.com/Schneegans/Burn-My-Windows/releases/latest/download/burn_my_windows_kwin4.tar.gz
mkdir -p ~/.local/share/kwin/effects
tar -xf burn_my_windows_kwin4.tar.gz -C ~/.local/share/kwin/effects
```
- Then select the desired effects in the system settings under "Desktop Effects".


#### Rounded Corners
https://github.com/matinlotfali/KDE-Rounded-Corners
```shell
sudo apt install git cmake g++ extra-cmake-modules kwin-dev libkf5configwidgets-dev 

git clone https://github.com/matinlotfali/KDE-Rounded-Corners
cd KDE-Rounded-Corners
mkdir build
cd build
cmake ..
cmake --build . -j
sudo make install

sh ../tools/load.sh
```



<br><br>
<br><br>

# Login Screen
- https://store.kde.org/p/1323349


<br><br>
<br><br>

# Wallpaper Enginge
- https://steamcommunity.com/workshop/browse/?appid=431960&browsesort=trend&section=readytouseitems

## Mobile
- If you can not connect to your host machine via your android phone then try to export mpkg:
- https://help.wallpaperengine.io/en/mobile/pairing-fixes.html#backup-solution-manually-importing-a-wallpaper-file-mpkg
  - I do not know where the file will be saved because it is proton from steam. However, re-open the process and then just copy the file from the file explorer

## Vertical search
- Go to settings and then Display choose `Scale and Crop`. And then choose any 4k wallpaper. Alternative you can go for this search:
  - https://steamcommunity.com/workshop/browse/?appid=431960&requiredtags[]=Portrait+1080+x+1920

## Best of
- https://steamcommunity.com/sharedfiles/filedetails/?id=1558194170
- https://steamcommunity.com/sharedfiles/filedetails/?id=2981249186
- https://steamcommunity.com/sharedfiles/filedetails/?id=2874353757

## KDE plugin 
- https://github.com/catsout/wallpaper-engine-kde-plugin

1. Download steam, go to Settings > Compatiblity > Run other titles with and choose `Proton Experimental`

2. Install Wallpaper enginge via steam and select some wallpaper via the launched app.

3. Install dependencies for ubuntu:
```
sudo apt install build-essential libvulkan-dev plasma-workspace-dev gstreamer1.0-libav \
liblz4-dev libmpv-dev python3-websockets qtbase5-private-dev \
libqt5x11extras5-dev \
qml-module-qtwebchannel qml-module-qtwebsockets cmake
```

4. Install plugin:
```
# Download source
git clone https://github.com/catsout/wallpaper-engine-kde-plugin.git
cd wallpaper-engine-kde-plugin

# Download submodule (glslang)
git submodule update --init

# Configure
# 'USE_PLASMAPKG=ON': using plasmapkg2 tool to install plugin
mkdir build && cd build
cmake .. -DUSE_PLASMAPKG=ON

# Build
make -j$nproc

# Install package (ignore if USE_PLASMAPKG=OFF for system-wide installation)
make install_pkg
# install lib
sudo make install
```

5. Then right click on your desktop and change wallpaper. Choose at `Wallpaper Type` then `Wallpaper KDE engine`
- Then click the library button and **navigate via your mouse** to the Path `~/.local/share/Steam`. Do not paste it or otherwhise it maybe not work.
- You maybe have to restart if you can not see any wallpapers yet `systemctl --user restart plasma-plasmashell.service`

6. I recommend to go to Settings tab and then choose 60 fps + Playback Speed 0.20


If wallpaper freezes try to restart plasma:
```shell
systemctl --user restart plasma-plasmashell.service
```


Also on every new screen or in general sometimes it may not working again then you may have to set again the steam folder again



<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>





















<br><br>

## Fedora
- ZSH (https://kifarunix.com/install-and-setup-zsh-and-oh-my-zsh-on-fedora-32/)

```bash
sudo dnf install make automake gcc gcc-c++ kernel-devel zsh
```

## Guides
- How to run GitLab in a docker container (https://www.youtube.com/watch?v=sLnbWGN77Uc)







<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>




# disable klipper (clipboard history)
- Of course you can disable it in the systray settings. (systray settings are the taskbar settings)
- Just untick the checkbox in "General"->"Extra Items".






<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>



# Pulse Effects
```bash
sudo apt install pulseeffects
```





<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>

# Firewall
- https://github.com/CyberT33N/ufw-cheat-sheet/blob/main/README.md

















<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>

<br><br>

#### Sandbox
- https://github.com/CyberT33N/firejail-cheat-sheet





































<br><br>
<br><br>
______________________________________________________________
<br><br>
<br><br>


#### KDE (Ubuntu)
```bash
sudo apt install kde-full

# later choose SDDM display manager

# Then reboot and in the login screen area choose PLASMA X11. For me it was like this on Ubuntu 22.04
```



<br><br>
<br><br>


#### KDE Themes
- System Settings > Appearance > Get new global themes
  - Daisy (https://store.kde.org/p/1597008)






<br><br>
<br><br>
______________________________________________________________
<br><br>
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

### Ubuntu
```bash
# Method #1

# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update

# Install latest version
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

# Verify that the Docker Engine installation is successful by running the hello-world image.
sudo docker run hello-world




# ----------------------------------------------


# Method #2
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt update
sudo apt install docker-ce
```

<br><br><br><br>


#### docker-compose
```
sudo apt install docker-compose
```




#### Docker Desktop
- https://docs.docker.com/desktop/install/ubuntu/

1. Set up Docker’s package repository.
2. Download latest DEB package.
3.Install the package with apt as follows:
```shell
sudo apt-get update
sudo apt-get install ./docker-desktop-<version>-<arch>.deb
```



















<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>

# Git

## git-tools
- https://github.com/T-vK/git-tools

<br><br>

## Enable some colorization of Git output.
```bash
git config --global color.ui auto
```

<br><br>

## SSH
- https://github.com/CyberT33N/git-cheat-sheet/blob/main/README.md#ssh

<br><br>

## Pushing to multiple git repos
- https://github.com/CyberT33N/git-cheat-sheet/blob/main/README.md#pushing-to-multiple-git-repos

<br><br>

## GUI
- GitKraken (PREMIUM - Cross Platform): https://www.gitkraken.com/download
- Sourcetree (FREE - Windows & MAC): https://www.sourcetreeapp.com/











<br><br>
 _____________________________________________________
 _____________________________________________________
<br><br>










































<br><br>
 _____________________________________________________
 _____________________________________________________

<br><br>


# Node.js 

## Windows
- https://nodejs.org/dist/v15.0.1/node-v15.0.1-x64.msi
- https://github.com/CyberT33N/nvm-cheat-sheet

<br><br><br><br>

## MAC
https://nodejs.org/dist/v15.0.1/node-v15.0.1.pkg

<br><br><br><br>

## Linux

#### NVM (https://github.com/nvm-sh/nvm)
- https://github.com/CyberT33N/nvm-cheat-sheet












































<br><br>
 _____________________________________________________
 _____________________________________________________

<br><br>

# Sublime

## How to install plugin??
```
# Press CTRL+SHift+P and then Enter
Install Package Control

Then search for your plugin and press Enter
```



























<br><br>
 _____________________________________________________
 _____________________________________________________

<br><br>

# Webstorm (https://www.jetbrains.com/de-de/webstorm/)
- https://github.com/CyberT33N/webstorm-cheat-sheet


















































<br><br>
 _____________________________________________________
 _____________________________________________________

<br><br>

# VS CODE
- https://github.com/CyberT33N/vs-code-cheat-sheet

























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

