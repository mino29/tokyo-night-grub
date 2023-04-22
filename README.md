# Tokyo-Night for [GRUB](https://gnu.org/software/grub/)

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)![Arch](https://img.shields.io/badge/Arch%20Linux-1793D1?logo=arch-linux&logoColor=fff&style=for-the-badge)

> A dark theme for [GRUB](https://gnu.org/software/grub/).
Basically just minor tweaks of Dracula grub that I made to go along with my
[arch i3 rice](https://github.com/mino29/arch-i3).

![Screenshot](./screenshot.png)

This can adapt to various resolustions of screens, at least my 1080p screen
worked just fine.

## Compatibility
> It should be compatible with all linux distros that uses grub

But I only used ubuntu, fedora and arch  so far, so your mileage may vary.

## Install

Steps:

1. clone this repo or download the .zip

```bash
git clone https://github.com/mino29/tokyo-night-grub.git
```

2. Change directory 

```
cd tokyo-night-grub
```

3. copy the whole tokyo-night directory grub themes

```bash
sudo cp -r tokyo-night /boot/grub/themes
```

4. edit grub file

```
sudo vim /etc/default/grub
```
change `#GRUB_THEME=` to
`GRUB_THEME="/boot/grub/themes/tokyo-night/theme.txt"`

5. use magic and reboot

run this command
```
sudo grub-mkconfig -o /boot/grub/grub.cfg
```
then reboot and voila

## Potential problems and solutions

Oh oh, can't see grub menu or boot into arch linux?

Grub on Arch Linux can be a pain to deal with recently.
After I change the theme and reboot and cannot boot into my Arch Linux, had to
do a "chroot", but worry not, here's what you need:

- USB drive with arch iso
- 15 minutes of free time
- Stable internet connection
- [this on-point article](https://www.jeremymorgan.com/tutorials/linux/how-to-reinstall-boot-loader-arch-linux/)


## Credit

- [Cute Ghost profile](https://www.flaticon.com/free-icon/ghost_1150381?term=ghost&page=1&position=52&page=1&position=52&related_id=1150381&origin=style)
- [Dracula Grub](https://draculatheme.com/grub)

## License

[MIT License](./LICENSE)
