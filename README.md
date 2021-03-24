## Clover Hackintosh Files

backup of my high sierra files, thou they shall not get lost

### What works

Everything except sleep.

Enable the "prevent computer from sleeping automatically when the display is off" option.

### Specs

These Clover files work with:

```bash
* CPU              Intel 7700K
* Mainboard        Gigabytes GA-B250M-D3H
* Graphics         NVIDIA GTX 1070
* RAM              16GB DDR4
* Storage          ADATA XPG SX8200 512GB
```

NVIDIA is not supported in newer macOS releases. :(

### Tipps

The HighSierra dmg will say that the install disk is damaged, open a terminal and change the date to fix this.

```bash
date -u 1010101017
```

When installing and updating it will crash mid installation once.

### Post-Installation

1. Update to the latest highSierra version
2. Reboot and check the OS build number by clicking on the macOS version in about
3. Install the fitting [nvidia driver](https://www.tonymacx86.com/nvidia-drivers/)
4. Reboot and disable automatic os and nvidia updates

Install Clover on your PC and change the boot order to your disk in the config.plist file and add a time out.

Happy hacking!
