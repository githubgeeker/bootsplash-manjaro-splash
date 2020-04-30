# Bootsplash-manjaro-splash

Another Bootsplash theme for manjaro Linux using White Manjaro logo

This project was based on multiple other great projects like:

https://github.com/Blacksuan19/Bootsplash-Themes

https://github.com/GrayJack/manjaro-grayjack/tree/master/PKGBUILDs/manjaro-bootsplash-green


Author: Pablo Lenna

# Installation:

- `git clone https://github.com/githubgeeker/bootsplash-manjaro-splash`
- `cd bootsplash-manjaro-splash`
- run `chmod +x bootsplash-manjaro-splash.sh`
- run `chmod +x bootsplash-packer`
- run `sh bootsplash-manjaro-splash.sh` to generate STL model.
- run `makepkg -s` to create an Arch package and install it with `pacman -U $package_name`or alternatively make and install with one single command: `makepkg -sci`
- append `bootsplash-manjaro-splash` hook at the end of HOOKS string in `/etc/mkinitcpio.conf`
- add `bootsplash.bootfile=bootsplash-themes/manjaro-splash/bootsplash` at the end of `GRUB_CMDLINE_LINUX` string in `/etc/default/grub` and don't forget to remove the `quiet` parameter!
- run `sudo mkinitcpio -P linux`
- run `sudo update-grub`
