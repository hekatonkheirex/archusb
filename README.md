# Hyprland-Arch Rice installed in a USB Drive
## My personal Hyprland config in a USB Drive
___
> ### <div align="center">*-- Disclaimer --*   </div>
> *I am not a developer/programmer, just a Linux enthusiast. All this configurations are just what I learned along the way by myself. You may encounter some redundant lines of code.*
___
<img src="https://i.imgur.com/nGGcmZY.png">

* **Distro** • [Arch Linux](https://archlinux.org/) 🐧
* **Window Manager** • [Hyprland](https://hyprland.org/) 💧
* **Colorscheme** • [Oxocarbon](https://github.com/nyoom-engineering/oxocarbon) 💻
  * **Backup Colorscheme** •  [Catppuccin](https://github.com/catppuccin) 🐈
* **Shell** • [Zsh](https://www.zsh.org) 🐚 with
  * [zinit](https://github.com/zdharma-continuum/zinit) 💤
  * [Starship](https://github.com/starship/starship) 🚀
* **Terminal** • [Kitty](https://sw.kovidgoyal.net/kitty/) 🐈
* **Panel** • [Waybar](https://github.com/Alexays/Waybar) 🍫
* **Notication Daemon** • [Swaync](https://github.com/ErikReider/SwayNotificationCenter) 🔔
* **Launcher** • [Rofi](https://github.com/davatorium/rofi) ⚓ with [rofimoji](https://github.com/fdw/rofimoji) 😐
* **File Manager** • [Thunar](https://docs.xfce.org/xfce/thunar/start) 🗄️
* **Music player** • [Spotify](https://open.spotify.com/) 🪕
* **Editor** • [Neovim](https://neovim.io/) 📝
  <details>
  <summary>Installed plugins</summary>
    * [LazyVim](https://www.lazyvim.org/)
  </details>  


* **Backup Editor** • [Visual Studio Code](https://code.visualstudio.com/) 📝
  <details>
  <summary>Installed plugins</summary>

     * [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
     * [Catppuccin for VSCode](https://marketplace.visualstudio.com/items?itemName=Catppuccin.catppuccin-vsc)
     * [Oxocarbon](https://marketplace.visualstudio.com/items?itemName=ibmlover.oxocarbon)
     * [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
     * [Django](https://marketplace.visualstudio.com/items?itemName=batisteo.vscode-django)
     * [Font Awesome Auto-complete & Preview](https://marketplace.visualstudio.com/items?itemName=Janne252.fontawesome-autocomplete)
     * [HTML CSS Support](https://marketplace.visualstudio.com/items?itemName=ecmel.vscode-html-css)
     * [Indenticator](https://marketplace.visualstudio.com/items?itemName=SirTori.indenticator)
     * [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
     * [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
     * [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
     * [Rasi](https://marketplace.visualstudio.com/items?itemName=dlasagno.rasi)
     * [Spanish - Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker-spanish)
     * [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)
  </summary>


## Before installation note
*You can review the `pkglist.txt` file to remove the packages you don't want and replace the ones you like, but I cannot guarantee if don't work as expected. Please, read the disclaimer*

## Installation
1. Do a fresh Arch Linux installation. *Remember to install `git` package during installation*. *You can also install on your existing installation, just skip to section 5*.
2. Install `paru`. *You can install whatever version you like, I prefer the binary version*. *You can also use whatever AUR helper you want, but remeber to uninstall `paru` at the end of the installation or remove the `paru-bin` line inside the `pkglist.txt` file*  
```
git clone https://aur.archlinux.org/paru-bin.git
cd paru-bin
makepkg -si
```  
3. Fork this repository or download it.  
4. If you forked it, use [yadm](https://yadm.io/) to download your forked repo.
  ```
  yadm clone https://github.com/youruser/yourforkedrepo.git
  ```  
5. If you downloaded it or cloned it, copy everything to your home directory (all the .config and .local directory, and all the *" . "* files as well).
6. Use `paru` (or the AUR helper of choice) to install everything in the `pkglist.txt` file. *You can use `pacman` too, but it won't install the AUR packages*.
```
paru -S --needed - < pkglist.txt
```  