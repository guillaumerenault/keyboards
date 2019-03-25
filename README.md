# Keyboards
My Keyboard configurations.


- **[Ergodox](#ergodox)**
<br/>

- **[History](./HISTORY.md)**
- **[Other settings](#other-settings)**


## Ergodox

- [General information](#ergodox-general-information)
- [OS layout](#ergodox-os-layout)
  - [Installation](#ergodox-os-layout-installation)
- [Physical layout](#ergodox-physical-layout)
- [Layout editors](#ergodox-layout-editors)
- [Flashing a layout](#ergodox-flashing-a-layout)
- [Hardware](#ergodox-hardware)
- [Known issues](#ergodox-known-issues)

<a id="ergodox-general-information"></a>
### General information
- [https://deskthority.net/wiki/ErgoDox](https://deskthority.net/wiki/ErgoDox)
- [https://www.ergodox.io/](https://www.ergodox.io/)

<a id="ergodox-os-layout"></a>
### OS layout

qwertyfr : [http://marin.jb.free.fr/qwerty-fr/](http://marin.jb.free.fr/qwerty-fr/)

<a id="ergodox-os-layout-installation"></a>
#### Installation

(Mirror from the qwerty-fr site)

- .deb packages based Linux
    - dpkg -i [.deb](./static/xkb-qwerty-fr_0.5_all.deb)
    - select Layout "English (US)" with variant "French (qwerty-fr; US with french symbols)"
- [Arch Linux](https://aur.archlinux.org/packages/xkb-qwerty-fr/)
- Mac OS
    - Download [tgz archive](./static/qwerty-fr_mac.tgz)
    - extract qwerty-fr.bundle to:
        - /Library/Keyboard Layouts/ to install for all users
        - ~/Library/Keyboard Layouts/ for user-local installation
- Windows
    - Download [zip archive](./static/win-qwerty-fr.zip)
    - extract files and run setup.exe
    - For default input language select "French (France) - French qwerty keyboard"

In case of other Linux distribution or installation issue, you can refer to [manual installation](http://marin.jb.free.fr/qwerty-fr/manual/) page for Linux.

<a id="ergodox-physical-layout"></a>
### Physical layout
Currently using only 2 layers :

layer0:
![layer0](./static/layer0.png "layer0")

layer1:
![layer1](./static/layer1.png "layer1")

- [.hex file](./layout_2019.03.25.hex)
- [source](./layout_2019.03.25)
- [editor](https://configure.ergodox-ez.com/layouts/Gzwa)

<a id="ergodox-layout-editors"></a>
### Layout editors
- Ergodox layout configurators :
  - Ergodox EZ (newer) : [https://configure.ergodox-ez.com](https://configure.ergodox-ez.com)
  - Massdrop : [https://www.massdrop.com/configurator/ergodox](https://www.massdrop.com/configurator/ergodox)

- Visual Layout Editor : [http://www.keyboard-layout-editor.com/](http://www.keyboard-layout-editor.com/)

<a id="ergodox-flashing-a-layout"></a>
### Flashing a layout
- Using the teensy loader cli:
 - [Official website](https://www.pjrc.com/teensy/loader_cli.html)
 - [Github](https://github.com/PaulStoffregen/teensy_loader_cli)

(The command I use for the teensy board I have)
```teensy_loader_cli -mmcu=atmega32u4 -w -v layout.hex```

<a id="ergodox-hardware"></a>
### Hardware
- Fully assembled MX-Brown switches Ergodox from fengsbay on ebay.
- Keycaps from https://pimpmykeyboard.com


![Ergodox](./static/ergodox.jpg "Ergodox")

<a id="ergodox-known-issues"></a>
### Known issues
- Windows 7
  - Key Chattering : [https://deskthority.net/wiki/Chatter](https://deskthority.net/wiki/Chatter)
    - [Fix](./issues/win7_key_chattering)

## Other settings
- [Xfce settings](./static/Xfce_settings.png)