 
# GRUB

## Useful resources
- [Virtuaverse grub theme](https://github.com/Patato777/dotfiles/tree/main/grub/themes/virtuaverse)

## Installation order
1. Copy the ./default folder to /etc/grub/default (you can do backup of the original default if you want to):
```bash
sudo mv /etc/default/grub /etc/default/grub.bak # make a backup
sudo cp ./default /etc/default/grub
```
2. Then copy ./themes folder to /efi/grub/themes (or efi dir you use):
```bash
sudo cp ./themes/ /efi/grub/themes
```

## Arch Linux with windows
I use arch linux in dual boot with windows, so [default/40_custom](default/40_custom) includes windows bootloader into grub. It has **_[REDACTED]_** which you can fix by doing:
```bash
cat /etc/fstab | sed -n "s/\(UUID=\)\(\S\+\)\(.*\/[efi|boot|boot\/efi]\+.*\)/\2/gp"
```
and copying the output

## nvidia, again
If you've read my dotfiles, you know I have to cope with shitty nvidia drivers. So you might occasionally see lines related to nvidia drivers config.

