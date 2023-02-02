HOW TO INSTALL DEBIAN OR LINUX

get a usb
get a terminal

run these cmds

mount /dev/sda1 /mnt
mv efi boot /mnt
sync
umount -f /mnt
mount /dev/sda2 /mnt
mv live /mnt/

boot from grub
