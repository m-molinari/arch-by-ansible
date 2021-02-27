# Configuring systems with ansible
Collection of system tools managed by ansible

# Basic Arch Installtion commands :
```bash

loadkeys it  

ip addr flush dev enp0s3  
ifconfig enp0s3 192.168.1.101 netmask 255.255.255.0  
route add default gw 192.168.1.1  
echo "nameserver 8.8.8.8" >> /etc/resolv.conf  

fdisk /dev/sdX  

1 /root  
2 swap  

mkfs.ext4 /dev/sda1  
mkswp /dev/sda2  

mount /dev/sda1 /mnt  
swapon /dev/sda2  

pacstrap /mnt base base-devel linux linux-firmware nano vim  
genfstab -U -p /mnt >> /mnt/etc/fstab  
arch-chroot /mnt /bin/bash  
ln -sf /usr/share/zoneinfo/Europe/Rome /etc/localtime  
hwclock --systohc  
echo arch > /etc/hostname  
vim /etc/hosts  
passwd  
echo "KEYMAP=it" > /etc/vconsole.conf  

pacman -S networkmanager dhcpcd net-tools  
systemctl enable NetworkManager  
systemctl enable dhcpcd  

passwd  
pacman -S grub  os-prober  
grub-install /dev/sda  
grub-mkconfig -o /boot/grub/grub.cfg  
 
pacman -S sudo bash-completion  
pacman -S git ansible  

useradd -m -g users -G wheel -s /bin/bash username  
passwd user  

pacman -S xorg-server xorg-xinit xorg-utils xorg-server-utils mesa xf86-input-synaptics  

```

# Virtualbox
```bash

pacman -S virtualbox-guest-utils virtualbox-guest-dkms virtualbox-guest-iso virtualbox-host-dkms  
systemctl enable vboxservice.service   
modprobe -a vboxguest vboxsf vboxvideo 

```


