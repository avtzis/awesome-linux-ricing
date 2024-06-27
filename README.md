<br/>
<div align='center'>
  <img src='media/awesome_tux.png'>
  <h1>Awesome Linux Ricing</h1>
  <h4>Carefully curated list of awesome Linux customization resources</h4>
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome Badage"></a>
</div>
<br/>
<p align="center">
	<a href="installation.md">Installation</a>&nbsp;&nbsp;•&nbsp;
	<a href="contributing.md">Contribution</a>&nbsp;&nbsp;•&nbsp;
	<a href="LICENSE">License</a>&nbsp;&nbsp;•&nbsp;
	<a href="code_of_conduct.md">Code of Conduct</a>
</p>
<br/>

## Description

This meticulously curated list is designed to assist users in personalizing their Linux desktop, a practice often referred to as 'ricing'. This resource compiles a carefully selected list of themes, tools, and customization options, offering users a comprehensive starting point for customizing their computers. Whether you seek common themes and tools or have specific preferences in mind, this repository provides a structured approach to explore and tailor your Linux desktop to your liking.


## Contents

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [GRUB](#grub)
- [Display Managers](#display-managers)
  - [sddm](#sddm)
  - [lightdm](#lightdm)
  - [gdm](#gdm)
- [Desktop Environments / Window Managers](#desktop-environments--window-managers)
  - [Classic/Stacking](#classicstacking)
  - [Tiling](#tiling)
  - [Dynamic (Stacking + Tiling)](#dynamic-stacking--tiling)
- [Themes](#themes)
  - [Utilities](#utilities)
- [Wallpapers](#wallpapers)
  - [Utilities](#utilities-1)
- [(Nerd) Fonts](#nerd-fonts)
- [Bar / Panel](#bar--panel)
- [Cursors](#cursors)
- [Icons](#icons)
- [App Launchers](#app-launchers)
- [Notifications](#notifications)
- [Widgets](#widgets)
- [Logout Menu](#logout-menu)
- [Screen Lock](#screen-lock)
- [Terminal](#terminal)
  - [Emulators](#emulators)
  - [Shell](#shell)
  - [Prompt](#prompt)
  - [Multiplexer](#multiplexer)
  - [Apps and Tools](#apps-and-tools)
  - [Fetches](#fetches)
  - [Fancies](#fancies)
- [UI Apps/Tools](#ui-appstools)
  - [Web Browsers](#web-browsers)
  - [File Managers](#file-managers)
  - [Image Viewers](#image-viewers)
  - [Music Players](#music-players)
  - [Video Streamers](#video-streamers)
  - [Document Readers](#document-readers)
  - [Text Editors](#text-editors)
  - [Archive Managers](#archive-managers)
  - [Email](#email)
  - [Calculators](#calculators)
  - [Notes](#notes)
  - [Workstation - Content Creation](#workstation---content-creation)
  - [Gaming](#gaming)
- [App Theming](#app-theming)
  - [Firefox](#firefox)
  - [Spotify](#spotify)
  - [Discord](#discord)
  - [VSCode](#vscode)
- [Installation](#installation)
- [Contribution](#contribution)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

---

## Window Managers
<details>
  <summary><b>Window Manager (WM) vs Desktop Environment (DE)</b></summary>
  <p>A <b>WM</b> is a software that manages the windows on your screen. It controls the placement and appearance of windows, and provides basic functionality like window resizing and moving.</p>
  <p>A <b>DE</b> is a collection of software that provides a complete desktop experience. It includes the <b>window manager</b>, along with a file manager, a bar/panel, and other apps, tools and utilities.</p>
  <p><b>DEs</b> usually provide a more integrated and user-friendly experience, while <b>WMs</b> are more lightweight and customizable, requiring you to manually configure and install additional software to get the same functionality as a <b>DE</b>, but with more control over the look and feel of your desktop.</p>
</details>
<br/>
<details>
  <summary><b>Stacking vs Tiling vs Dynamic WMs</b></summary>
  <ul>
    <li><b>Stacking WMs</b> are traditional window managers that place windows on top of each other (like MS Windows). They allow you to move and resize windows freely, but they can be cluttered and hard to manage with many windows open.</li>
    <li><b>Tiling WMs</b> automatically arrange windows in a non-overlapping layout. They are efficient and help you make the most of your screen space, but they can be less flexible than stacking WMs.</li>
    <li><b>Dynamic WMs</b> combine the best of both worlds. They allow you to switch between tiling and stacking layouts, giving you the flexibility to choose the best layout for your workflow.</li>
  </ul>
</details>
<br/>
<details>
  <summary><b>X11 vs Wayland</b></summary>
  <p><b>X11</b> is the traditional display server protocol used in Linux. It is mature and stable, but it has some limitations in terms of security and performance.</p>
  <p><b>Wayland</b> is a newer display server protocol that aims to address the limitations of <b>X11</b>. It is more secure and efficient, allowing for better performance, smoother animations, touch gestures, etc. However, it is still under development, and usually Nvidia GPUs have issues with it.</p>
  <p>All applications with a GUI (as well as WMs) are run under a display server and are usually developed for a specific display server protocol, meaning you can't run a <b>Wayland</b> app on <b>X11</b>, or vice versa. However, it is possible to use a compatibility layer like XWayland to run <b>X11</b> apps on <b>Wayland</b>.</p>
</details>
<br/>

### Stacking

- [GNOME](https://gitlab.gnome.org/GNOME)<sup>X11 + Wayland</sup> - A modern desktop environment that aims to be simple and easy to use.
- [KDE](https://kde.org/)<sup>X11 + Wayland</sup> - A feature-rich and versatile desktop environment.
- [XFCE](https://www.xfce.org/)<sup>X11</sup> - A lightweight desktop environment. It aims to be fast and low on system resources, while still being visually appealing and user-friendly.
- [Openbox](http://openbox.org/)<sup>X11</sup> - A highly configurable next generation window manager with extensive standards support.


### Tiling

- [bspwm](https://github.com/baskerville/bspwm)<sup>X11</sup> - A tiling window manager that represents windows as the leaves of a full binary tree.
- [i3](https://github.com/i3/i3)<sup>X11</sup> - A tiling window manager for X11.
- [sway](https://github.com/swaywm/sway)<sup>Wayland</sup> - Α tiling Wayland compositor and a drop-in replacement for the i3 window manager for X11.
- [herbstluftwm](https://github.com/herbstluftwm/herbstluftwm)<sup>X11</sup> - A manual tiling window manager for X.


### Dynamic

- [Ηyprland](https://github.com/hyprwm/Hyprland)<sup>Wayland</sup> - Α highly customizable dynamic tiling Wayland compositor that doesn't sacrifice on its looks.
- [awesome](https://github.com/awesomeWM/awesome)<sup>X11</sup> - A highly configurable, next generation framework window manager for X.
- [QTile](https://github.com/qtile/qtile)<sup>X11 + Wayland</sup> - A full-featured, hackable tiling window manager.
- [XMonad](https://github.com/xmonad/xmonad)<sup>X11</sup> - Α small but functional ICCCM-compliant tiling window manager.
- [dwm](https://dwm.suckless.org/)<sup>X11</sup> - Α dynamic window manager for X. It manages windows in tiled, monocle and floating layouts.
- [river](https://github.com/riverwm/river)<sup>Wayland</sup> - Α dynamic tiling Wayland compositor with flexible runtime configuration.
- [ragnar](https://github.com/cococry/ragnar)<sup>X11</sup> - Minimal, flexible & user-friendly X tiling window manager.


## Color Schemes

<details>
  <summary><b>What are color schemes</b></summary>
  wip
</details>
<br/>

- [Catppuccin](https://github.com/catppuccin/catppuccin) - Soothing pastel theme for the high-spirited.
- [Gruvbox](https://github.com/morhetz/gruvbox) - Retro groove color scheme.
- [Nord](https://github.com/nordtheme/nord) - Arctic, north-bluish color palette.
- [Everforest](https://github.com/sainnhe/everforest) - Comfortable and pleasant green forest color scheme.
- [Dracula](https://github.com/dracula/dracula-theme) - Dark spooky theme.
- [Rosé Pine](https://github.com/rose-pine/rose-pine-theme) - All natural pine, faux fur and a bit of soho vibes for the classy minimalist.
- [Tokyo Night](https://github.com/enkia/tokyo-night-vscode-theme#other-ports) - Clean, dark theme that celebrates the lights of Tokyo at night.
- [Sweet](https://github.com/EliverLara/Sweet) - Colorful candy theme.
- [Kanagawa](https://github.com/rebelot/kanagawa.nvim) - Dark color scheme inspired by the famous painting.
- [BlackLotus](https://github.com/PoisonIsBestType/BlackLotus) - Dark, dim, blue, purple... beautiful.
- [Whale](https://github.com/anufrievroman/whale) - Dark theme inspired by Ark and Nord.
- [Everblush](https://github.com/Everblush/everblush) - Dark, vibrant and beautiful Colorscheme.
- [Shades of purple](https://github.com/EliverLara/Shades-of-purple-gtk) - Sweet purple theme.
- [opulo](https://github.com/kewmine/opulo) - Colorscheme for absolute nerds.
- [camellia](https://github.com/camellia-theme/camellia) - Dark yet vibrant color scheme.

### Utilities

- [pywall](https://github.com/dylanaraps/pywal) - Generate and change color-schemes according to your wallpaper.
- [wpgtk](https://github.com/deviantfero/wpgtk) - A colorscheme, wallpaper and template manager.


## Wallpapers

Some great repos with wallpaper collections by:
- [dharmx](https://github.com/dharmx/walls)
- [linuxdotexe](https://github.com/linuxdotexe/nordic-wallpapers)<sup>Nord</sup>
- [D3Ext](https://github.com/D3Ext/aesthetic-wallpapers)
- [FrenzyExists](https://github.com/FrenzyExists/wallpapers)
- [AngelJumbo](https://github.com/AngelJumbo/gruvbox-wallpapers)<sup>Gruvbox</sup>
- [Gingeh](https://github.com/Gingeh/wallpapers)<sup>Catppuccin</sup>
- [Apeiros-46B](https://github.com/Apeiros-46B/everforest-walls)<sup>Everforest</sup>
- [gboncoffee](https://github.com/gboncoffee/wallpapers)
- [zDyanTB](https://github.com/zDyanTB/aesthetic-wallpapers)
- [vctrblck](https://github.com/vctrblck/gruvbox-wallpapers)<sup>Gruvbox</sup>
- [jorgeloopzz](https://github.com/jorgeloopzz/Wallpapers)
- [Axenide](https://github.com/Axenide/Wallpapers)


### Utilities

- [swww](https://github.com/Horus645/swww)<sup>Wayland</sup> - Efficient animated wallpaper daemon for wayland, controlled at runtime.
- [mpvpaper](https://github.com/GhostNaN/mpvpaper)<sup>Wayland</sup> - A video wallpaper program for wlroots based wayland compositors.
- [swaybg](https://github.com/swaywm/swaybg)<sup>Wayland</sup> - Wallpaper tool for Wayland compositors
- [hyprpaper](https://github.com/hyprwm/hyprpaper)<sup>Wayland</sup> - A fast Wayland wallpaper utility with IPC controls.


## Fonts
<details>
  <summary><b>What is the difference between Sans, Serif and Mono</b></summary>
  <ul>
    <li><b>Serif</b> fonts have decorative lines or strokes at the ends of the letters. They are often used for body text in printed materials.</li>
    <li><b>Sans-serif</b> fonts are modern and clean, without the decorative flourishes of serif fonts. They are often used for headings and titles.</li>
    <li><b>Monospace</b> fonts have equal spacing between characters, making them ideal for coding, editors and terminals.</li>
  </ul>
    <p><b>Sans</b> and <b>Mono</b> are the ones usually used for ricing, as they are more readable and modern.</p>
</details>
<br/>

### Sans Fonts
- [Google Sans](https://font.download/font/google-sans)
- [Open Sans](https://fonts.google.com/specimen/Open+Sans)
- [Roboto](https://fonts.google.com/specimen/Roboto)
- [Ubuntu](https://fonts.google.com/specimen/Ubuntu)

### Monospace Fonts
- [JetBrains Mono](https://github.com/JetBrains/JetBrainsMono) - ligatures
- [FiraCode](https://github.com/tonsky/FiraCode) - ligatures
- [Cascadia Code](https://github.com/microsoft/cascadia-code) - ligatures
- [Iosevka](https://github.com/be5invis/Iosevka) - ligatures
- [Victor Mono](https://github.com/rubjo/victor-mono) - ligatures
- [DejaVu](https://github.com/dejavu-fonts/dejavu-fonts)
- [Gohufont](https://github.com/hchargois/gohufont)
- [Operator-caska Cursive](https://github.com/Anant-mishra1729/Operator-caska-Font#operator-caska-cursive-font)

### Nerd Fonts
<details>
  <summary><b>What are the Nerd Fonts</b></summary>
    <b>Nerd Fonts</b> are patched fonts that contain additional glyphs, icons, and ligatures. These fonts are designed to be used in terminals and code editors, providing a more visually appealing and functional experience. <b>Nerd Fonts</b> are compatible with most of the font families.
</details>
<br/>

- [Nerd Fonts](https://github.com/ryanoasis/nerd-fonts) - Collection of nerd fonts.
- [font-patcher](https://github.com/ryanoasis/nerd-fonts?tab=readme-ov-file#font-patcher) - Patch your own fonts.
- [getnf](https://github.com/getnf/getnf) - A helpful tool to install Nerd Fonts.

## Bar / Panel
- [Polybar](https://github.com/polybar/polybar)<sup>X11</sup>
- [Waybar](https://github.com/Alexays/Waybar)<sup>Wayland</sup>
- [Eww](https://github.com/elkowar/eww)<sup>X11 + Wayland</sup>
- [ags](https://github.com/Aylur/ags)<sup>X11 + Wayland</sup>
- [lemonbar](https://github.com/LemonBoy/bar)<sup>X11</sup>
- [gBar](https://github.com/scorpion-26/gBar)<sup>Wayland</sup>
- [fabric](https://github.com/Fabric-Development/fabric/)<sup>X11 + Wayland</sup>


## Cursors

- [Bibata](https://github.com/ful1e5/Bibata_Cursor)
- [BreezeX](https://github.com/ful1e5/BreezeX_Cursor)
- [Qogir](https://github.com/vinceliuice/Qogir-icon-theme)
- [Apple](https://github.com/ful1e5/apple_cursor)
- [Fuchsia](https://github.com/ful1e5/fuchsia-cursor)


## Icons

- [Candy](https://github.com/EliverLara/candy-icons)
- [Papirus](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme)
- [Tela](https://github.com/vinceliuice/Tela-icon-theme)
- [BeautyLine](https://github.com/gvolpe/BeautyLine)
- [Flat Remix](https://github.com/daniruiz/Flat-Remix)
- [Qogir](https://github.com/vinceliuice/Qogir-icon-theme)


## App Launchers

- [Rofi](https://github.com/davatorium/rofi)
	- [custom configs](https://github.com/adi1090x/rofi) - by adi1090x
- [Ulauncher](https://github.com/Ulauncher/Ulauncher/)
- [Anyrun](https://github.com/Kirottu/anyrun)
- [Gauntlet](https://github.com/project-gauntlet/gauntlet)


## Notifications

- [Dunst](https://github.com/dunst-project/dunst)
- [SwayNC](https://github.com/ErikReider/SwayNotificationCenter)
- [mako](https://github.com/emersion/mako)

## Widgets

- [conky](https://github.com/brndnmtthws/conky) - System monitoring.
- [GLava](https://github.com/jarcode-foss/glava) - Audio spectrum visualizer.
- [Kando](https://github.com/kando-menu/kando) - The Cross-Platform Pie Menu.
- [wallpaper-cava](https://github.com/rs-pro0/wallpaper-cava) - Display cava on top of your wallpaper.


## Logout Menu

- [wlogout](https://github.com/ArtsyMacaw/wlogout)


## Screen Lock

- [swaylock](https://github.com/swaywm/swaylock) - for Wayland
- [hyprlock](https://github.com/hyprwm/hyprlock)


## Terminal

### Emulators

- [kitty](https://github.com/kovidgoyal/kitty)
- [alacritty](https://github.com/alacritty/alacritty)
- [st](https://github.com/siduck/st)
- [foot](https://codeberg.org/dnkl/foot)
- [wezterm](https://github.com/wez/wezterm)


### Shell

- [zsh](https://zsh.sourceforge.io/)
  - [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)
  - [prezto](https://github.com/sorin-ionescu/prezto)
  - [Antigen](https://github.com/zsh-users/antigen)
  - [zimfw](https://github.com/zimfw/zimfw)
  - [zinit](https://github.com/zdharma-continuum/zinit)
  - [zsh4humans](https://github.com/romkatv/zsh4humans)
  - [zap](https://github.com/zap-zsh/zap)
  - [zgen](https://github.com/tarjoilija/zgen)
- [fish](https://github.com/fish-shell/fish-shell)
- [nushell](https://github.com/nushell/nushell)


### Prompt

- [Starship](https://github.com/starship/starship)
- [oh-my-posh](https://github.com/JanDeDobbeleer/oh-my-posh)
- [powerlevel10k](https://github.com/romkatv/powerlevel10k) - zsh
- [Pure](https://github.com/sindresorhus/pure) - zsh
- [roundy](https://github.com/nullxception/roundy) - zsh


### Multiplexer
  - [tmux](https://github.com/tmux/tmux)
  - [zellij](https://github.com/zellij-org/zellij)
  - [byobu](https://www.byobu.org/home)
  - [screen](https://www.gnu.org/software/screen/)


### Apps and Tools

- File Managers
  - [ranger](https://github.com/ranger/ranger)
    - [devicons](https://github.com/alexanderjeurissen/ranger_devicons)
  - [yazi](https://github.com/sxyazi/yazi)
  - [superfile](https://github.com/yorukot/superfile)
- Editors
  - [vim](https://github.com/vim/vim)
  - [neovim](https://github.com/neovim/neovim)
  - [nano](https://github.com/madnight/nano)
  - [Helix](https://github.com/helix-editor/helix)
  - [micro](https://github.com/zyedidia/micro)
- Image Viewers
  - [catimg](https://github.com/posva/catimg)
  - [timg](https://github.com/hzeller/timg)
  - [imcat](https://github.com/stolk/imcat)
- Music Streamers
  - [cmus](https://github.com/cmus/cmus)
  - [ncmpcpp](https://github.com/ncmpcpp/ncmpcpp) - [MPD](https://github.com/MusicPlayerDaemon/MPD)
  - [spotify-tui](https://github.com/Rigellute/spotify-tui) - spotify
  - [spotify_player](https://github.com/aome510/spotify-player) - spotify
- System Monitoring
  - [btop](https://github.com/aristocratos/btop)
  - [htop](https://github.com/htop-dev/htop)
  - [Glances](https://github.com/nicolargo/glances)
  - [s-tui](https://github.com/amanusk/s-tui)
- IRC Clients
  - [WeeChat](https://github.com/weechat/weechat)
  - [irssi](https://github.com/irssi/irssi)
- Mail Clients
  - [mutt](https://gitlab.com/muttmua/mutt)
- Screenshot
  - [scrot](https://github.com/resurrecting-open-source-projects/scrot)
- Recording
  - [wf-recorder](https://github.com/ammen99/wf-recorder)
- Directory Listing
  - [lsd](https://github.com/Peltoche/lsd)
  - [exa](https://github.com/ogham/exa)
  - [logo-ls](https://github.com/Yash-Handa/logo-ls)
  - [Color LS](https://github.com/athityakumar/colorls)
- Misc
  - [evillimiter](https://github.com/bitbrute/evillimiter) - Tool that monitors, analyzes and limits the bandwidth of devices on the local network without administrative access.
  - [carbon-now-cli](https://github.com/mixn/carbon-now-cli) - Beautiful images of your code — from right inside your terminal.
  - [nvm](https://github.com/nvm-sh/nvm) - POSIX-compliant bash script to manage multiple active node.js versions.
  - [xdg-ninja](https://github.com/b3nj5m1n/xdg-ninja) - A shell script which checks your $HOME for unwanted files and directories.
  - [ncdu](https://code.blicky.net/yorhel/ncdu) - A disk usage analyzer with an ncurses interface.
  - [arch-update](https://github.com/Antiz96/arch-update) - An update applier for Arch Linux that assists you with important pre/post update tasks.
- more:
  - [awesome-cli-apps](https://github.com/agarrharr/awesome-cli-apps)
  - [awesome-shell](https://github.com/alebcay/awesome-shell)

### Fetches

- [neofetch](https://github.com/dylanaraps/neofetch)
  - [themes](https://github.com/Chick2D/neofetch-themes)
- [pfetch](https://github.com/dylanaraps/pfetch)
- [fastfetch](https://github.com/fastfetch-cli/fastfetch)
- [ufetch](https://gitlab.com/jschx/ufetch)
- [bunnyfetch](https://github.com/Rosettea/bunnyfetch)
- [uwufetch](https://github.com/ad-oliviero/uwufetch)
- [rxfetch](https://github.com/Mangeshrex/rxfetch)
- [nerdfetch](https://github.com/ThatOneCalculator/NerdFetch)
- [nitch](https://github.com/ssleert/nitch)
- [macchina](https://github.com/Macchina-CLI/macchina/)
- [hyfetch](https://github.com/hykilpikonna/hyfetch)

### Fancies

#### Terminal Visuals
- [pipes.sh](https://github.com/pipeseroni/pipes.sh) - Animated pipes terminal screensaver.
- [cbonsai](https://gitlab.com/jallbrit/cbonsai) - Grow bonsai trees in your terminal.
- [Shell Color Scripts](https://gitlab.com/dwt1/shell-color-scripts) - A collection of terminal color scripts.
- [Asciiquarium](https://github.com/cmatsuoka/asciiquarium) - Enjoy the mysteries of the sea from the safety of your own terminal!
- [ascii-rain](https://github.com/nkleemann/ascii-rain) - Ncurses rain effect.
- [Nyancat](https://github.com/klange/nyancat) - Nyancat in your terminal, rendered through ANSI escape sequences.
- [SL](https://github.com/mtoyoda/sl) - SL(1): Cure your bad habit of mistyping.
- [arttime](https://github.com/poetaman/arttime) - text art with functionality of clock / timer / pattern-based time manager.
- [sortty](https://github.com/dormant-chicken/sortty) - Sorting algorithms in the terminal.

#### Clocks
- [tty-clock](https://github.com/xorg62/tty-clock) - Clock using lib ncurses.
- [Peaclock](https://github.com/octobanana/peaclock) - A responsive and customizable clock for the terminal.

#### Audio Visualizers
- [CAVA](https://github.com/karlstav/cava) - Cross-platform Audio Visualizer.
- [Musializer](https://github.com/tsoding/musializer) - Music Visualizer.
- [ReVidia](https://github.com/GhostNaN/ReVidia-Audio-Visualizer) - A highly customizable real time audio visualizer.
- [ReCidia](https://github.com/GhostNaN/recidia-audio-visualizer) - A highly customizable real time audio visualizer on Linux.

#### Matrix
- [CMatrix](https://github.com/abishekvashok/cmatrix) - Terminal based "The Matrix" like implementation.
- [neo](https://github.com/st3w/neo) - Simulates the digital rain from "The Matrix".
- [unimatrix](https://github.com/will8211/unimatrix) - Python script to simulate the display from "The Matrix" in terminal.

#### Character Play
- [cowsay](https://github.com/piuccio/cowsay) - A configurable talking cow.
- [lovesay](https://github.com/dotzenith/lovesay.rs) - Cowsay, but full of love.
- [ponysay](https://github.com/erkin/ponysay) - Pony rewrite of cowsay.
- [boxes](https://github.com/ascii-boxes/boxes/) - Command line ASCII boxes unlimited!
- [fortune](http://bxr.su/OpenBSD/games/fortune/) - Random poignant, inspirational, silly or snide phrases.

#### Pokemon-Themed
- [pokemon-colorscripts](https://gitlab.com/phoneybadger/pokemon-colorscripts) - CLI utility to print out images of pokemon to terminal.
- [pokeget-rs](https://github.com/talwat/pokeget-rs) - A bash script you can use to display cool sprites of pokemon in your terminal.
- [pokeshell](https://github.com/acxz/pokeshell) - A featureful shell program to show pokemon sprites in the terminal.
- [krabby](https://github.com/yannjor/krabby) - Print pokemon sprites in your terminal.
- [Poketex](https://github.com/ckaznable/poketex) - Simple Pokedex based on TUI.

#### Text and Fonts
- [FIGlet](https://github.com/cmatsuoka/figlet) - Claudio's FIGlet tree.
- [toilet](https://github.com/cacalabs/toilet) - The Other Implementation of figLET.
- [lolcat](https://github.com/busyloop/lolcat) - Rainbows and unicorns!
- [lolcrab](https://github.com/mazznoer/lolcrab) - Like lolcat but with noise and more colorful.



## UI Apps/Tools

### Web Browsers

- [Firefox](https://www.mozilla.org/firefox)
- [chromium](https://github.com/chromium/chromium)
- [Brave](https://github.com/brave/brave-browser)
- [Tor](https://www.torproject.org/)
- [thorium](https://github.com/Alex313031/Thorium)
- [Floorp](https://github.com/Floorp-Projects/Floorp/)

### File Managers

- [Nemo](https://github.com/linuxmint/nemo)
- [Nautilus](https://gitlab.gnome.org/GNOME/nautilus)
- [Dolphin](https://invent.kde.org/system/dolphin)
- [thunar](https://gitlab.xfce.org/xfce/thunar)
- [PCmanFM](https://github.com/lxde/pcmanfm)

### Image Viewers

- [imv](https://git.sr.ht/~exec64/imv)
- [feh](https://github.com/derf/feh)
- [Eye of GNOME](https://gitlab.gnome.org/GNOME/eog)

### Music Players

- [Amberol](https://gitlab.gnome.org/World/amberol)
- [DeaDBeeF](https://github.com/DeaDBeeF-Player/deadbeef)
- [Sunamu](https://github.com/NyaomiDEV/Sunamu)
- [feishin](https://github.com/jeffvli/feishin)
- [G4Music](https://github.com/neithern/g4music)
- [lyssa](https://github.com/cococry/lyssa)

### Video Streamers

- [VLC](https://github.com/videolan/vlc)
- [mpv](https://github.com/mpv-player/mpv)

### Document Readers

- [zathura](https://git.pwmt.org/pwmt/zathura)
- [Bookworm](https://github.com/babluboy/bookworm)

### Text Editors

- [gedit](https://gitlab.gnome.org/GNOME/gedit)
- [geany](https://github.com/geany/geany)
- [kate](https://github.com/KDE/kate)
- [vscodium](https://github.com/VSCodium/vscodium) - VSCode without spying.

### Archive Managers

- [File Roller](https://gitlab.gnome.org/GNOME/file-roller)

### Email

- [Thunderbird](https://github.com/mozilla/releases-comm-central)

### Calculators

- [GNOME Calculator](https://gitlab.gnome.org/GNOME/gnome-calculator)


### Notes

- [Obsidian](https://obsidian.md/) - NOT open-source


### Workstation - Content Creation

- Image Editors
  - [GIMP](https://gitlab.gnome.org/GNOME/gimp)
- Video Editors
  - [Kdenlive](https://invent.kde.org/multimedia/kdenlive)
  - [DaVinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve) - NOT open-source
- Music
  - [Blue](https://github.com/kunstmusik/blue)
  - [MuseScore](https://github.com/musescore/MuseScore)
- 3D
  - [blender](https://github.com/blender/blender)
- Office
  - [LibreOffice](https://github.com/LibreOffice/core)
- Screen Recording / Live Streaming
  - [OBS Studio](https://github.com/obsproject/obs-studio)

### Gaming

- [Steam](https://github.com/ValveSoftware/steam-for-linux) - [Proton](https://github.com/ValveSoftware/Proton) - [Wine](https://github.com/ValveSoftware/wine)
- [Lutris](https://github.com/lutris/lutris)
- [Heroic](https://github.com/Heroic-Games-Launcher/HeroicGamesLauncher)
- [Cartridges](https://github.com/kra-mo/cartridges)


## App Theming

### Firefox

- Themes
  - [Sweet](https://github.com/EliverLara/firefox-sweet-theme)
  - [Nord](https://github.com/EliverLara/firefox-nordic-theme)
  - [Cascade](https://github.com/andreasgrafen/cascade)
  - [Mod-Blur](https://github.com/datguypiko/Firefox-Mod-Blur)
  - [Onebar](https://codeberg.org/Freeplay/Firefox-Onebar)
  - [penguinFox](https://github.com/p3nguin-kun/penguinFox)
  - [FlyingFox](https://github.com/akshat46/FlyingFox)
  - [SimpleFox](https://github.com/migueravila/SimpleFox)
  - [ShyFox](https://github.com/Naezr/ShyFox)
- Startpage
  - [dawn](https://github.com/b-coimbra/dawn)
  - [Excalith](https://github.com/excalith/excalith-start-page)
  - [yags](https://github.com/PrettyCoffee/yet-another-generic-startpage)
  - [Bento-next](https://github.com/lewisdoesstuff/bento-next)
  - [Starter Tab](https://github.com/allister-grange/startertab)
  - [nightTab](https://github.com/zombieFox/nightTab)


### Spotify

- [Spicetify](https://github.com/spicetify/spicetify-cli) - [themes](https://github.com/spicetify/spicetify-themes)

### Discord

- [BetterDiscord](https://github.com/BetterDiscord/BetterDiscord) - [themes](https://betterdiscord.app/themes)
- [Vencord](https://github.com/Vendicated/Vencord)

### VSCode

- [Tokyo Night](https://github.com/enkia/tokyo-night-vscode-theme)


## Display Managers

- [sddm](https://github.com/sddm/sddm)
  - [Sugar Dark](https://github.com/MarianArlt/sddm-sugar-dark)
  - [Tokyo Night](https://github.com/rototrash/tokyo-night-sddm)
  - [Sugar Candy](https://framagit.org/MarianArlt/sddm-sugar-candy)
  - [LentenRose](https://github.com/theoisdumb/lentenrose)
  - [corners](https://github.com/aczw/sddm-theme-corners)
- [lightdm](https://github.com/canonical/lightdm)
  - [Shikai](https://github.com/TheWisker/Shikai)
  - [Web Greeter](https://github.com/JezerM/web-greeter)
- [gdm](https://gitlab.gnome.org/GNOME/gdm)
- [ly](https://github.com/fairyglade/ly)


## GRUB

<details>
  <summary><b>What is GRUB</b></summary>
    <b>GRUB</b> (GRand Unified Bootloader) is a versatile bootloader commonly used in Linux distributions. It's the software that you first see when your computer starts, allowing you to select which operating system or kernel to boot into. <b>GRUB</b> is very customizable and there is plenty of creative themes made by users.
</details>
<br/>

- [grub2-themes](https://github.com/vinceliuice/grub2-themes) - Modern design GRUB theme collection.
- [Matter](https://github.com/mateosss/matter) - Customizable GRUB theme inspired by Material Design.
- [Dark Matter](https://github.com/VandalByte/darkmatter-grub2-theme) - Dark Matter GRUB Theme.
- [Tartarus](https://github.com/AllJavi/tartarus-grub) - Basic grub theme with material gruvbox style.
- [Dracula](https://github.com/dracula/grub) - Dracula GRUB theme.
- [Tokyo Night](https://github.com/mino29/tokyo-night-grub) - A GRUB theme using Tokyo Night color scheme based on Dracula GRUB.
- [Poly dark](https://github.com/shvchk/poly-dark) -  Poly dark GRUB theme.
- [Minegrub](https://github.com/Lxtharia/minegrub-theme) -  A GRUB theme in Minecraft style.

> [!TIP]
> To install a theme, follow the instructions provided in the respective theme's  repo.

---

## Installation
The majority of these items are linked to their corresponding repositories. Please endeavor to find installation instructions within these repositories. Additionally, it's *strongly* advisable to explore your distribution's package manager to see if a pre-packaged solution is available. **PROTIP**: It's best to refrain from using the "download" button on Linux.

## Contribution
Any helpful contribution is welcome, especially for original content!

<!-- ### Thanks -->


