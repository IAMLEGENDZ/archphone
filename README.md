# ArchPhone

A project what aims to get GNOME Shell, Arch Linux and Wayland working on Android tablets/phones natively (no chroot)

Current status: __Researching and testing stuff__

Updates: Got new phone and got bored so I decided to continue

# Why? There is Ubuntu Touch already!
Actually, Ubuntu Touch gave me an idea for this.

I would like to run normal desktop apps with my phone, but that seems impossible on Ubuntu Touch.

# Initial project goals
- ~~Research how does Android boot.~~ DONE
- ~~Do some research at Google Nexus 5 drivers and kernel.~~ Everything else except Wifi seems tricky
- ~~Build serial debug cable~~ Needs proper schematic, but I can live without it atm
- ~~Install Arch Linux into LXC on Android~~ FAIL, can't get android compiler working
- ~~Get Arch Linux installed on Google Nexus 7 (2012)~~
- Get Arch Linux installed on Google Nexus 5 and get display working
- Run Weston with freedreno driver
- Usable GNOME DE (with keyboard and mouse at first place)
- Install Chromium and things I normally use
- Get 3.17+ kernel or TSYNC patch to make Chromium usable. [See this](http://www.phoronix.com/scan.php?page=news_item&px=Google-Chrome-TSYNC-Kernel)
- 3G Networking

# Ideas for later
- Touchscreen here I come
- MultiROM package, not tutorial how to replace Android
- XWayland
- Get camera and bluetooth working (libhybris??)
- Make kernel only to boot into Arch Linux (Android features removed)
- Get 4G and SMS working (but no calling)
- On-screen keyboard maybe?
- Release images (fastboot packages)

## Things that could stop or slow down this project:
- Binary wifi/BT/camera drivers
- ~~Audio (audio didn't work on Ubuntu, so it's very unlikely I get it working)~~ _carmine_ sent me a nice e-mail, and said that audio is working (yay!)
- ~~systemd wants pretty new kernel (I don't remember from head, but 3.4.x is too old) (I can set pacman to hold systemd package)~~ Seems like Android kernel got many backported stuff. systemd runsn even on Nexus7 kernel (which is 3.1.x)
- no info for Freedreno on Nexus 5 !! or if Freedreno works, I can run only older Xorg

## Things what are bad, but won't slow down this project:
- Desktop apps are bit big for phones.
- I don't know how libhybris actually works!

## Useful things:
- [KDE Plasma MultiROM image](https://community.kde.org/Plasma/Mobile/MultiROM) (tested on Nexus 5)
- Nexus 6 3.10 kernel: http://goo.gl/uHhDzb
- Nexus 4 Fedora: https://github.com/freedreno/nexus4-fedora *CHROOT*
- Android boot: http://elinux.org/Android_Booting
- Freedreno: https://github.com/freedreno/freedreno
- If I ever need Mali GPU driver: http://limadriver.org/
- libhybris: https://github.com/libhybris/libhybris
- Gentoo on TF201: https://wiki.gentoo.org/wiki/Asus_Transformer_Prime
- Any linux distro on TF201: http://lifeinarootshell.blogspot.it/2013/03/howto.html
- Nokia N900 Arch Linux: https://github.com/archlinuxarm-n900
- Ubuntu Touch and Android on LXC: https://wiki.ubuntu.com/Touch/ContainerArchitecture
- Arch Linux on Nexus 7 2013: https://github.com/crondog/arch-flo
- Arch Linux on Nexus 7 2012: https://docs.google.com/document/d/1G9vF5v2TN2c6ocyb_hmD1ve7OK4GdCP84rfaXgiLmB4/edit?pli=1 
