# REALTEK RTL88x2B USB Linux Driver  
**Current Driver Version**: 5.8.7.1  
**Support Kernel**: 2.6.24 ~ 5.8 (with unofficial patches)  

Official release note please check ReleaseNotes.pdf  

**Note:** if you believe your device is **RTL8812BU** or **RTL8822BU** but after loaded the module no NIC shows up, the device ID maybe not in the driver whitelist. In this case please submit a new issue with `lsusb` result, and your device name, brand, website, etc.

## Added Supported Devices
* RaspBerry Pi 4B(Linux raspberrypi 5.4.51-v7l+ #1333 SMP Mon Aug 10 16:51:40 BST 2020 armv7l GNU/Linux)

## Supported Devices
* ASUS AC1300 USB-AC55 B1
* ASUS U2
* Dlink - DWA-181
* Dlink - DWA-182
* Edimax EW-7822ULC
* Edimax EW-7822UTC
* NetGear A6150
* TP-Link Archer T3U
* TP-Link Archer T3U Plus
* TP-Link Archer T4U V3
* TRENDnet TEW-808UBM

And more.

# How to use this kernel module
* Make sure you have installed the kernel headers
* All commands need to be run in the driver directory
* The following commands only build module for the current running kernel
* You need rebuild the kernel module everytime you update/change the kernel

## Building && Installing
```
apt update
apt upgrade
apt dist-upgrade
apt-get install libelf-dev
apt install make
apt install make-guile
apt install gcc  dkms
apt-get install libncurses5-dev
git clone https://github.com/MyDynasty/RTL88x2BU-Linux-Driver.git
cd RTL88x2BU-Linux-Driver
apt-get install bc
make
make install
reboot
```

## Uninstalling
```
sudo make uninstall
```

# USB 3.0 Support
You can try use `modprobe 88x2bu rtw_switch_usb_mode=1` to force the adapter run under USB 3.0. But if your adapter/port/motherboard not support it, the driver will be in restart loop. Remove the parameter and reload the driver to restore.

# Distribution
* Archlinux AUR https://aur.archlinux.org/packages/rtl88x2bu-dkms-git/
