Debian 11

Graphics addapter
=================

To have your graphics addapter recognized and working at full resolution install
a different kernel version from the Debian Backports repository. The entire sequence
of steps is the following:

1) Configure the Backports repository in your apt system.

   Add the following two lines to the /etc/apt/sources.list file

   deb http://deb.debian.org/debian bullseye-backports main contrib non-free
   deb-src http://deb.debian.org/debian bullseye-backports main contrib non-free

2) Run apt-get update

   $ apt-get update

3) Install the new kernel

   apt-get install linux-image-5.19.0-0.deb11.2-amd64


Bluetooth addapter
==================

To activate the bluetooth addapter on this motherboard install the following package

apt-get install firmware-iwlwifi 

Wireless addapter
==================

The wireless addapter worked when we tried to use it. We have tried
it after the backports kernel linux-image-5.19.0-0.deb11.2-amd64 was
installed so we do not know if the wireless addapter works  with the
original kernel or if the backports kernel is required. The wireless
antenna provided with the motherboard must be connected.

Audio addapter
==============

Works with the kernel linux-image-5.19.0-0.deb11.2-amd64 available from backports.



