# NVIDIA
![Linus Torvalds, the creator of Linux, showing middle finger to nvidia](https://i.imgur.com/hdJi6r9.jpeg)

I don't have money or need to upgrade my PC so I have to cope with those shitty drivers.

## Useful resources
- [Korvahannu driver installation guide](https://github.com/korvahannu/arch-nvidia-drivers-installation-guide)
- [Arch driver installation guide](https://wiki.archlinux.org/title/NVIDIA)
- Might be helpful: [Lutris docs driver installation](https://github.com/lutris/docs/blob/master/InstallingDrivers.md)

## Installation order
1. Copy the nvidia hooks into pacman hooks folder:
```bash
sudo cp ./nvidia.hook /etc/pacman.d/hooks/
```
2. Follow the useful resources. Don't copy or write nvidia.hook by hand as you've already copied it.
