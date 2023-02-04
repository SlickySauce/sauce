#!/bin/sh
sudo apt-get install python pkg-config bison flex
sudo apt-get install autoreconf autogen
tar -xf grub-2.06.tar.gz
./autogen.sh
./bootstrap
./configure.sh
make
make install
cp -R include/* /usr/include/
cp config.h /usr/include/
cp config.h /usr/include/grub/
cp config-util.h /usr/include/grub/
cp config-util.h /usr/include/
apt-get install qemu
grub-mkimage -o grub.img -O i386-pc -p .
qemu-system-i386 --kernel grub.img
exit 0;

