TL-WN725N-V2-Driver-for-Linux
=============================

TL-WN725N V2 Driver for Linux 

Support Linux 3.7.0-

Support Linux 3.7.0+ (tested)

Install
=======

1. Prepare linux-headers

1. Get source code from Github

	`git clone https://github.com/twd2/TL-WN725N-V2-Driver-for-Linux.git`

1. Make
	
	`cd TL-WN725N-V2-Driver-for-Linux`

	`zcat /proc/config.gz > .config`

	`make`

1. Install

	```install 8188eu.ko /lib/modules/`uname -r`/kernel/net/wireless/```

	`depmod -a`

	`modprobe -i 8188eu`

1. Configure as usual


Reference
=========

1. https://github.com/liwei/rpi-rtl8188eu

1. https://realtek-8188cus-wireless-drivers-3444749-ubuntu-1304.googlecode.com/

1. http://gencarelle.com/blog/2013/07/19/problems-with-rtl8188cus/
