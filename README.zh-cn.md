# REALTEK RTL88x2B USB Linux Driver  
**Current Driver Version**: 5.8.7.1  
**Support Kernel**: 2.6.24 ~ 5.8 (with unofficial patches)  



## 无线网卡版本

```
Realtek Semiconductor Corp. USB3.0 802.11ac 1200M Adapter
Realtek 8812BU Wireless LAN 802.11ac USB NIC
```

## 系统内核版本
```bash
pi@raspberrypi:~ $ uname -r
5.4.51-v7l+
```

# 食用方式


```bash
pi@raspberrypi:~ $ sudo apt-get update
pi@raspberrypi:~ $ sudo apt-get upgrade
pi@raspberrypi:~ $ sudo apt dist-upgrade

pi@raspberrypi:~ $ sudo apt-get install libelf-dev
pi@raspberrypi:~ $ sudo apt install make
pi@raspberrypi:~ $ sudo apt install make-guile
pi@raspberrypi:~ $ sudo apt install gcc  dkms
pi@raspberrypi:~ $ sudo apt-get install libncurses5-dev libncursesw5-dev

pi@raspberrypi:~ $ git clone https://github.com/MyDynasty/RTL88x2BU-Linux-Driver.git
pi@raspberrypi:~ $ cd RTL88x2BU-Linux-Driver
pi@raspberrypi:~ $ su root
root@raspberrypi:~/RTL88x2BU-Linux-Driver# apt-get update
root@raspberrypi:~/RTL88x2BU-Linux-Driver# apt-get install bc
root@raspberrypi:~/RTL88x2BU-Linux-Driver# make
root@raspberrypi:~/RTL88x2BU-Linux-Driver# make install
root@raspberrypi:~/RTL88x2BU-Linux-Driver# reboot
```
