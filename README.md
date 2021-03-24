## Clover Hackintosh Files

backup of my high sierra files, thou they shall not get lost

this will get deleted if apple ever makes hackintoshes illegal.

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

You can safely create a bootable usb stick with [tinu v.2.1](https://github.com/ITzTravelInTime/TINU/releases/download/2.1_PUBLIC_60/TINU.zip).

Use [Clover v.5108](https://github.com/CloverHackyColor/CloverBootloader/releases/download/5108/Clover_r5108.pkg) to install the bootloader on the created usb stick (check the custom option to install in EFI). This is the last and best version that will work with these files.

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
