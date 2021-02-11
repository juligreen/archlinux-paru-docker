## Image

This is a fork of the [archlinux-yay](https://hub.docker.com/r/oblique/archlinux-yay) docker image.

Docker image of [ArchLinux](https://www.archlinux.org) with [paru](https://github.com/Morganamilo/paru) installed.

## Usage

Install package from official repositories:

```
pacman --noconfirm -S <package>
```

Install package from AUR:

```
sudo -u aur paru --noconfirm -S <package>
```

Cleanup:

```
pacman -Qtdq | xargs -r pacman --noconfirm -Rcns
rm -rf /home/aur/.cache
```
