# ArchPhone
[Reddit link](http://www.reddit.com/r/linux/comments/30iydm/arch_linux_on_mobile_phones_idea/)

A project what aims to get GNOME Shell, Arch Linux and Wayland working on Android tablets/phones natively (no chroot)

# Why? There is Ubuntu Touch already!
Actually, Ubuntu Touch gave me an idea for this.

I would like to run normal desktop apps with my phone, but that seems impossible on Ubuntu Touch.

# Initial project goals
- ~~Research how does Android boot.~~ DONE
- ~~Do some research at Google Nexus 5 drivers and kernel.~~ Everything else except Wifi seems tricky
- ~~Build serial debug cable~~ Needs proper schematic, but I can live without it atm
- Get Arch Linux installed on Google Nexus 5 and get display working
- Run Weston with freedreno driver
- Usable GNOME DE (with keyboard and mouse at first place)
- Install Chromium and things I normally use
- Get 3.17+ kernel or TSYNC patch to make Chromium useable. [See this](http://www.phoronix.com/scan.php?page=news_item&px=Google-Chrome-TSYNC-Kernel)
- 3G Networking

# Ideas for later
- Touchscreen here I come
- XWayland
- Get camera and bluetooth working (libhybris??)
- Make kernel only to boot into Arch Linux (Android features removed)
- Get 4G and SMS working (but no calling)
- On-screen keyboard maybe?
- Release images (fastboot packages)

## Things that could stop or slow down this project:
- Binary wifi/BT/camera drivers
- Audio (audio didn't work on Ubuntu, so it's very unlikely I get it working)
- systemd wants pretty new kernel (I don't remember from head, but 3.4.x is too old) (I can set pacman to hold systemd package)
- no info for Freedreno on Nexus 5 !!

## Things what are bad, but won't slow down this project:
- Desktop apps are bit big for phones.
- I don't know how libhybris actually works!

## Useful things:
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
