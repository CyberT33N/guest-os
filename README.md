# Guest OS
List for software/dependencies for any guest OS when you want to start developing.. As example for companies..


<br><br>

# Cross Platform
- KeePassXC - Cross-Platform Password Manager (https://keepassxc.org/download/)
- Gitlab Docker (https://hub.docker.com/r/gitlab/gitlab-ce)

<br><br>

## Chromium

#### Extension
- Script Safe (https://chrome.google.com/webstore/detail/scriptsafe/oiigbmnaadbkfbmpbfijlflahbdbdgdf)
- Webrtc Anti Leak Prevent (https://chrome.google.com/webstore/detail/webrtc-leak-prevent/eiadekoaikejlgdbkbdfeijglgfdalml)
- Nimbus (https://chrome.google.com/webstore/detail/nimbus-screenshot-screen/bpconcjcammlapcogcnnelfmaeghhagj/related)











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
- https://starship.rs/
```shell
curl -sS https://starship.rs/install.sh | sh

sudo gedit ~/.zshrc
eval "$(starship init zsh)"

mkdir -p ~/.config && touch ~/.config/starship.toml
```


<br><br>
<br><br>


## Design #1
- https://i.redd.it/u86x4e91gju91.png
```toml
# Warning: This config does not include keys that have an unset value

# $all is shorthand for $username$hostname$localip$shlvl$singularity$kubernetes$directory$vcsh$git_branch$git_commit$git_state$git_metrics$git_status$hg_branch$docker_context$package$cmake$cobol$dart$deno$dotnet$elixir$elm$erlang$golang$haskell$helm$java$julia$kotlin$lua$nim$nodejs$ocaml$perl$php$pulumi$purescript$python$rlang$red$ruby$rust$scala$swift$terraform$vlang$vagrant$zig$buf$nix_shell$conda$memory_usage$aws$gcloud$openstack$azure$env_var$crystal$custom$sudo$cmd_duration$line_break$jobs$battery$time$status$container$shell$character
format = '$all'
right_format = ''
continuation_prompt = '[∙](bright-black) '
scan_timeout = 30
command_timeout = 500
add_newline = true

[aws]
format = 'on [$symbol($profile )(\($region\) )(\[$duration\])]($style)'
symbol = '☁️  '
style = 'bold yellow'
disabled = false
expiration_symbol = 'X'

[aws.region_aliases]

[aws.profile_aliases]

[azure]
format = 'on [$symbol($subscription)]($style) '
symbol = 'ﴃ '
style = 'blue bold'
disabled = true

[battery]
full_symbol = ' '
charging_symbol = ' '
discharging_symbol = ' '
unknown_symbol = ' '
empty_symbol = ' '
disabled = false
format = '[$symbol$percentage]($style) '

[[battery.display]]
threshold = 10
style = 'red bold'

[buf]
format = 'with [$symbol ($version)]($style)'
version_format = 'v${raw}'
symbol = ''
style = 'bold blue'
disabled = false
detect_extensions = []
detect_files = [
    'buf.yaml',
    'buf.gen.yaml',
    'buf.work.yaml',
]
detect_folders = []

[character]
format = '$symbol '
success_symbol = '[╰─>](bold cyan)'
error_symbol = '[╰─](bold red)[×](bold red)'
disabled = false

[cmake]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '△ '
style = 'bold blue'
disabled = false
detect_extensions = []
detect_files = [
    'CMakeLists.txt',
    'CMakeCache.txt',
]
detect_folders = []

[cobol]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '⚙️ '
style = 'bold blue'
disabled = false
detect_extensions = [
    'cbl',
    'cob',
    'CBL',
    'COB',
]
detect_files = []
detect_folders = []

[cmd_duration]
show_milliseconds = true
format = "took [$duration](bold yellow) "
disabled = true
show_notifications = true

[conda]
truncation_length = 1
format = 'via [$symbol$environment]($style) '
symbol = '🅒 '
style = 'green bold'
ignore_base = true
disabled = false

[container]
format = '[$symbol \[$name\]]($style) '
symbol = '⬢'
style = 'red bold dimmed'
disabled = false

[crystal]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🔮 '
style = 'bold red'
disabled = false
detect_extensions = ['cr']
detect_files = ['shard.yml']
detect_folders = []

[dart]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🎯 '
style = 'bold blue'
disabled = false
detect_extensions = ['dart']
detect_files = [
    'pubspec.yaml',
    'pubspec.yml',
    'pubspec.lock',
]
detect_folders = ['.dart_tool']

[deno]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🦕 '
style = 'green bold'
disabled = false
detect_extensions = []
detect_files = [
    'deno.json',
    'deno.jsonc',
    'mod.ts',
    'deps.ts',
    'mod.js',
    'deps.js',
]
detect_folders = []

[directory]
truncation_length = 3
truncate_to_repo = true
fish_style_pwd_dir_length = 0
use_logical_path = true
format = '[$path](bold #89dceb)[$read_only](bold yellow) '
repo_root_format = '[$before_root_path]($style)[$repo_root]($repo_root_style)[$path]($style)[$read_only]($read_only_style) '
style = 'bold underline'
disabled = false
read_only = ' 🔒'
read_only_style = 'red'
truncation_symbol = ''
home_symbol = '~'
use_os_path_sep = true

[directory.substitutions]

[docker_context]
symbol = '🐳 '
style = 'blue bold'
format = 'via [$symbol$context]($style) '
only_with_files = true
disabled = false
detect_extensions = []
detect_files = [
    'docker-compose.yml',
    'docker-compose.yaml',
    'Dockerfile',
]
detect_folders = []

[dotnet]
format = 'via [$symbol($version )(🎯 $tfm )]($style)'
version_format = 'v${raw}'
symbol = '.NET '
style = 'blue bold'
heuristic = true
disabled = false
detect_extensions = [
    'csproj',
    'fsproj',
    'xproj',
]
detect_files = [
    'global.json',
    'project.json',
    'Directory.Build.props',
    'Directory.Build.targets',
    'Packages.props',
]
detect_folders = []

[elixir]
format = 'via [$symbol($version \(OTP $otp_version\) )]($style)'
version_format = 'v${raw}'
symbol = '💧 '
style = 'bold purple'
disabled = false
detect_extensions = []
detect_files = ['mix.exs']
detect_folders = []

[elm]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🌳 '
style = 'cyan bold'
disabled = false
detect_extensions = ['elm']
detect_files = [
    'elm.json',
    'elm-package.json',
    '.elm-version',
]
detect_folders = ['elm-stuff']

[env_var]

[erlang]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = ' '
style = 'bold red'
disabled = false
detect_extensions = []
detect_files = [
    'rebar.config',
    'erlang.mk',
]
detect_folders = []

[fill]
style = 'bold black'
symbol = '.'
disabled = false

[gcloud]
format = 'on [$symbol$account(@$domain)(\($region\))]($style) '
symbol = '☁️  '
style = 'bold blue'
disabled = false

[gcloud.region_aliases]

[gcloud.project_aliases]

[git_branch]
format = 'on [$symbol$branch]($style)(:[$remote]($style)) '
symbol = ' '
style = 'bold purple'
truncation_length = 9223372036854775807
truncation_symbol = '…'
only_attached = false
always_show_remote = false
ignore_branches = []
disabled = false

[git_commit]
commit_hash_length = 7
format = '[\($hash$tag\)]($style) '
style = 'green bold'
only_detached = true
disabled = false
tag_symbol = ' 🏷  '
tag_disabled = true

[git_metrics]
added_style = 'bold green'
deleted_style = 'bold red'
only_nonzero_diffs = true
format = '([+$added]($added_style) )([-$deleted]($deleted_style) )'
disabled = true

[git_state]
rebase = 'REBASING'
merge = 'MERGING'
revert = 'REVERTING'
cherry_pick = 'CHERRY-PICKING'
bisect = 'BISECTING'
am = 'AM'
am_or_rebase = 'AM/REBASE'
style = 'bold yellow'
format = '\([$state( $progress_current/$progress_total)]($style)\) '
disabled = false

[git_status]
format = '([\[$all_status$ahead_behind\]]($style) )'
style = 'red bold'
stashed = '\$'
ahead = '⇡'
behind = '⇣'
up_to_date = ''
diverged = '⇕'
conflicted = '='
deleted = '✘'
renamed = '»'
modified = '!'
staged = '+'
untracked = '?'
ignore_submodules = false
disabled = false

[golang]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🐹 '
style = 'bold cyan'
disabled = false
detect_extensions = ['go']
detect_files = [
    'go.mod',
    'go.sum',
    'glide.yaml',
    'Gopkg.yml',
    'Gopkg.lock',
    '.go-version',
]
detect_folders = ['Godeps']

[haskell]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = 'λ '
style = 'bold purple'
disabled = false
detect_extensions = [
    'hs',
    'cabal',
    'hs-boot',
]
detect_files = [
    'stack.yaml',
    'cabal.project',
]
detect_folders = []

[helm]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '⎈ '
style = 'bold white'
disabled = false
detect_extensions = []
detect_files = [
    'helmfile.yaml',
    'Chart.yaml',
]
detect_folders = []

[hg_branch]
symbol = ' '
style = 'bold purple'
format = 'on [$symbol$branch]($style) '
truncation_length = 9223372036854775807
truncation_symbol = '…'
disabled = true

[hostname]
ssh_only = false
trim_at = '.'
format = '[$hostname](#94e2d5) in '
style = 'bold'
disabled = false

[java]
disabled = false
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
style = 'red dimmed'
symbol = '☕ '
detect_extensions = [
    'java',
    'class',
    'jar',
    'gradle',
    'clj',
    'cljc',
]
detect_files = [
    'pom.xml',
    'build.gradle.kts',
    'build.sbt',
    '.java-version',
    'deps.edn',
    'project.clj',
    'build.boot',
]
detect_folders = []

[jobs]
threshold = 1
symbol_threshold = 1
number_threshold = 2
format = '[$symbol$number]($style) '
symbol = '✦'
style = 'bold blue'
disabled = true

[julia]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = 'ஃ '
style = 'bold purple'
disabled = false
detect_extensions = ['jl']
detect_files = [
    'Project.toml',
    'Manifest.toml',
]
detect_folders = []

[kotlin]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🅺 '
style = 'bold blue'
kotlin_binary = 'kotlin'
disabled = false
detect_extensions = [
    'kt',
    'kts',
]
detect_files = []
detect_folders = []

[kubernetes]
symbol = '☸ '
format = '[$symbol$context( \($namespace\))]($style) in '
style = 'cyan bold'
disabled = true

[kubernetes.context_aliases]

[line_break]
disabled = false

[localip]
ssh_only = true
format = '[$localipv4]($style) '
style = 'yellow bold'
disabled = true

[lua]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🌙 '
style = 'bold blue'
lua_binary = 'lua'
disabled = false
detect_extensions = ['lua']
detect_files = ['.lua-version']
detect_folders = ['lua']

[memory_usage]
threshold = 75
format = 'via $symbol[$ram( | $swap)]($style) '
style = 'white bold dimmed'
symbol = '🐏 '
disabled = true

[nim]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '👑 '
style = 'yellow bold'
disabled = false
detect_extensions = [
    'nim',
    'nims',
    'nimble',
]
detect_files = ['nim.cfg']
detect_folders = []

[nix_shell]
format = 'via [$symbol$state( \($name\))]($style) '
symbol = '❄️  '
style = 'bold blue'
impure_msg = 'impure'
pure_msg = 'pure'
disabled = false

[nodejs]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = ' '
style = 'bold green'
disabled = false
not_capable_style = 'bold red'
detect_extensions = [
    'js',
    'mjs',
    'cjs',
    'ts',
    'mts',
    'cts',
]
detect_files = [
    'package.json',
    '.node-version',
    '.nvmrc',
]
detect_folders = ['node_modules']

[ocaml]
format = 'via [$symbol($version )(\($switch_indicator$switch_name\) )]($style)'
version_format = 'v${raw}'
global_switch_indicator = ''
local_switch_indicator = '*'
symbol = '🐫 '
style = 'bold yellow'
disabled = false
detect_extensions = [
    'opam',
    'ml',
    'mli',
    're',
    'rei',
]
detect_files = [
    'dune',
    'dune-project',
    'jbuild',
    'jbuild-ignore',
    '.merlin',
]
detect_folders = [
    '_opam',
    'esy.lock',
]

[openstack]
format = 'on [$symbol$cloud(\($project\))]($style) '
symbol = '☁️  '
style = 'bold yellow'
disabled = false

[package]
format = 'is [$symbol$version]($style) '
symbol = '📦 '
style = '208 bold'
display_private = false
disabled = false
version_format = 'v${raw}'

[perl]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🐪 '
style = '149 bold'
disabled = false
detect_extensions = [
    'pl',
    'pm',
    'pod',
]
detect_files = [
    'Makefile.PL',
    'Build.PL',
    'cpanfile',
    'cpanfile.snapshot',
    'META.json',
    'META.yml',
    '.perl-version',
]
detect_folders = []

[php]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🐘 '
style = '147 bold'
disabled = false
detect_extensions = ['php']
detect_files = [
    'composer.json',
    '.php-version',
]
detect_folders = []

[pulumi]
format = 'via [$symbol($username@)$stack]($style) '
version_format = 'v${raw}'
symbol = ' '
style = 'bold 5'
disabled = false

[purescript]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '<=> '
style = 'bold white'
disabled = false
detect_extensions = ['purs']
detect_files = ['spago.dhall']
detect_folders = []

[python]
pyenv_version_name = false
pyenv_prefix = 'pyenv '
python_binary = [
    'python',
    'python3',
    'python2',
]
format = 'via [${symbol}${pyenv_prefix}(${version} )(\($virtualenv\) )]($style)'
version_format = 'v${raw}'
style = 'yellow bold'
symbol = '🐍 '
disabled = false
detect_extensions = ['py']
detect_files = [
    'requirements.txt',
    '.python-version',
    'pyproject.toml',
    'Pipfile',
    'tox.ini',
    'setup.py',
    '__init__.py',
]
detect_folders = []

[red]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🔺 '
style = 'red bold'
disabled = false
detect_extensions = [
    'red',
    'reds',
]
detect_files = []
detect_folders = []

[rlang]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
style = 'blue bold'
symbol = '📐 '
disabled = false
detect_extensions = [
    'R',
    'Rd',
    'Rmd',
    'Rproj',
    'Rsx',
]
detect_files = ['.Rprofile']
detect_folders = ['.Rproj.user']

[ruby]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '💎 '
style = 'bold red'
disabled = false
detect_extensions = ['rb']
detect_files = [
    'Gemfile',
    '.ruby-version',
]
detect_folders = []
detect_variables = [
    'RUBY_VERSION',
    'RBENV_VERSION',
]

[rust]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🦀 '
style = 'bold red'
disabled = false
detect_extensions = ['rs']
detect_files = ['Cargo.toml']
detect_folders = []

[scala]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
disabled = false
style = 'red bold'
symbol = '🆂 '
detect_extensions = [
    'sbt',
    'scala',
]
detect_files = [
    '.scalaenv',
    '.sbtenv',
    'build.sbt',
]
detect_folders = ['.metals']

[shell]
format = '[$indicator]($style) '
bash_indicator = 'bsh'
fish_indicator = 'fsh'
zsh_indicator = 'zsh'
powershell_indicator = 'psh'
ion_indicator = 'ion'
elvish_indicator = 'esh'
tcsh_indicator = 'tsh'
nu_indicator = 'nu'
xonsh_indicator = 'xsh'
cmd_indicator = 'cmd'
unknown_indicator = ''
style = 'white bold'
disabled = true

[shlvl]
threshold = 2
format = '[$symbol$shlvl]($style) '
symbol = '↕️  '
repeat = false
style = 'bold yellow'
disabled = true

[singularity]
symbol = ''
format = '[$symbol\[$env\]]($style) '
style = 'blue bold dimmed'
disabled = false

[status]
format = '[$symbol$status]($style) '
symbol = '✖'
success_symbol = ''
not_executable_symbol = '🚫'
not_found_symbol = '🔍'
sigint_symbol = '🧱'
signal_symbol = '⚡'
style = 'bold red'
map_symbol = false
recognize_signal_code = true
pipestatus = false
pipestatus_separator = '|'
pipestatus_format = '\[$pipestatus\] => [$symbol$common_meaning$signal_name$maybe_int]($style)'
disabled = true

[sudo]
format = '[as $symbol]($style)'
symbol = '🧙 '
style = 'bold blue'
allow_windows = false
disabled = true

[swift]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '🐦 '
style = 'bold 202'
disabled = false
detect_extensions = ['swift']
detect_files = ['Package.swift']
detect_folders = []

[terraform]
format = 'via [$symbol$workspace]($style) '
version_format = 'v${raw}'
symbol = '💠 '
style = 'bold 105'
disabled = false
detect_extensions = [
    'tf',
    'tfplan',
    'tfstate',
]
detect_files = []
detect_folders = ['.terraform']

[time]
format = 'at [$time]($style) '
style = 'bold yellow'
use_12hr = false
disabled = true
utc_time_offset = 'local'
time_range = '-'

[username]
format = '[╭─](#b4befe)[$user](#b4befe)[@](bold)'
style_root = 'bold'
style_user = 'bold'
show_always = true
disabled = false

[vagrant]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '⍱ '
style = 'cyan bold'
disabled = false
detect_extensions = []
detect_files = ['Vagrantfile']
detect_folders = []

[vcsh]
symbol = ''
style = 'bold yellow'
format = 'vcsh [$symbol$repo]($style) '
disabled = false

[vlang]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = 'V '
style = 'blue bold'
disabled = false
detect_extensions = ['v']
detect_files = [
    'v.mod',
    'vpkg.json',
    '.vpkg-lock.json',
]
detect_folders = []

[zig]
format = 'via [$symbol($version )]($style)'
version_format = 'v${raw}'
symbol = '↯ '
style = 'bold yellow'
disabled = false
detect_extensions = ['zig']
detect_files = []
detect_folders = []

[custom]
```


<br><br>
<br><br>


# Fonts
- https://www.nerdfonts.com/font-downloads


<br><br>
<br><br>

# System details in terminal
```
sudo apt install neofetch
```

<br><br>
<br><br>


# KDE

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

The following code will not allow traffic from your own device e.g. WLAN/LAN to any other Port than DNS (53), local (192.168.0.0/16), NORDVPN(51820) & OPENVPN (1197). 

If connected to VPN we will allow only http, https & DNS:
```shell
sudo ufw reset
sudo ufw enable

# ---------------------------

# =====================
# ====== GLOBAL =======
# =====================

# Deny all
sudo ufw default deny forward
sudo ufw default deny incoming
sudo ufw default deny outgoing

# ---------------------------

# =====================
# ====== VPN ==========
# =====================

# If you want to allow any outgoing port
# sudo ufw allow out on nordlynx

# Allow only http, https & DNS
sudo ufw allow out on nordlynx to any port 80,443,53,8080 proto tcp
sudo ufw allow out on nordlynx to any port 80,443,53,8080 proto udp


# ---------------------------

# =====================
# ====== WLAN =========
# =====================

# Allow outgoing traffic from your device to DNS (53), NORDVPN(51820) & OPENVPN (1197)
sudo ufw allow out on wlp0s20f3 to any port 53,51820,1197 proto udp

# Allow NTP
# sudo ufw allow out on wlp0s20f3 to any port 123 proto udp comment 'allow NTP'

# Allow local networks (optional)
sudo ufw allow out on wlp0s20f3 to 192.168.0.0/16 comment 'allow local network'

# ---------------------------

sudo ufw status verbose
sudo ufw enable
```
- If it is not working and you can not connect to your vpn then try check_
  ```shell
  netstat -u
  netstat -t

  ```


If needed this code is a basic example for only enable http, https & DNS to your WLAN/LAN:
```shell
# Reset all Rules
sudo ufw reset

# ---------------------

# Enable Firewall
sudo ufw enable

# ---------------------

# deny all
sudo ufw default deny forward
sudo ufw default deny outgoing
sudo ufw default deny incoming

# ---------------------

# thunderbird
# sudo ufw allow 993

# thunderbird gmail send
# sudo ufw allow out 465

# thunderbird hotmail send
# sudo ufw allow out 587

# thunderbird
# sudo ufw allow out 993

# ---------------------

# qbittorrent
# sudo ufw allow 6969
# sudo ufw allow out 6969

# ---------------------

# dns
sudo ufw allow out 53

# ---------------------

# https & https
sudo ufw allow out http
sudo ufw allow out https
```






<br><br>
<br><br>
___________________________________
___________________________________
<br><br>
<br><br>

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

<br><br>

#### Recommended
- It is recommend to download srwiron .deb file and install it with sudo dpkg -i xxx.deb
  -  Then create chrome.profile file as related to my firejail cheat sheet from above. Create shortcut as related to this guide (https://github.com/CyberT33N/linux-cheat-sheet/blob/main/README.md#create-custom-shortcut-with-termainl-command):
    ```
    touch ~/Desktop/iron.desktop
    
    sudo nano ~/Desktop/iron.desktop
    
    #!/usr/bin/env xdg-open
    [Desktop Entry]
    Name=Iron [Sandboxed]
    Exec=/bin/bash -c "firejail /usr/share/iron/chrome"
    Type=Application
    Terminal=true
    Icon=/home/t33n/Downloads/chromium-logo.png
    ```
    - Use this Browser als sandboxed on for untrusted stuff.
      - Install firefox via snap install firefox and use it as your main browser without resitrictions

<br><br>

#### firejail all paramater
https://firejail.wordpress.com/features-3/man-firejail/







































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
sudo apt-get update
sudo apt-get install ca-certificates curl gnupg

sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg

echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
sudo docker run hello-world






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
- If you encounter error like nvm: install v18.16.0 failed! try:
```
sudo apt install build-essential
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

## Plugins
- Monokai Pro Theme(https://plugins.jetbrains.com/plugin/13643-monokai-pro-theme)
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

## Increae search limit results from 100 to xxxx
- In 2021.2 the limit is configurable in Settings | Advanced Settings | Maximum number of results to show in Find In Path/Show Usages preview.


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
- https://gist.github.com/CyberT33N/ef2ae6684f29734ba2263d07fe1548e7 **FINAL almost like atom v2**
- https://gist.github.com/CyberT33N/a3905f0b9da8cebb42d03998d79b6a5f **FINAL almost like atom**
- 
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

