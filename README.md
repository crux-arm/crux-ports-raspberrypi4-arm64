# crux-ports-raspberrypi3-arm64

CRUX-ARM aarch64 ports overlay for RaspberryPi 3

To use these ports, download the `raspberrypi3-arm64.httpup` file to `/etc/ports`:
```
$ sudo wget -P /etc/ports https://raw.githubusercontent.com/crux-arm/crux-ports-raspberrypi3-arm64/main/raspberrypi3-arm64.httpup
$ sudo ports -u raspberrypi3-arm64
```

You may want to list it first in `/etc/prt-get.conf` to take advantage of ports overlay:
```
###
### prt-get conf
###

# note: the order matters: the package found first is used
prtdir /usr/ports/raspberrypi3-arm64
prtdir /usr/ports/core-arm64
prtdir /usr/ports/opt-arm64
prtdir /usr/ports/xorg-arm64
prtdir /usr/ports/core
prtdir /usr/ports/opt
prtdir /usr/ports/xorg
```
