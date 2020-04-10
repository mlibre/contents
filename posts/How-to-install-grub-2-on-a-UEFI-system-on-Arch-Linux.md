# How to install grub 2 on a UEFI system on Arch Linux

[![How to install grub 2 on a UEFI system on Arch Linux](http://img.youtube.com/vi/EDx7PhDBP-o/0.jpg)](https://www.youtube.com/watch?v=EDx7PhDBP-o "How to install grub 2 on a UEFI system on Arch Linux")


Install grub 2 on a UEFI system, EFI partition, on Arch Linux<br/>Commands:<br/>sudo pacman -S grub efibootmgr<br/>sudo mount /dev/sdxx /mnt # sdxx is your EFI partition.<br/>sudo grub-install --target=x86_64-efi --efi-directory=/mnt --bootloader-id=grub --recheck<br/>sudo grub-mkconfig -o /boot/grub/grub.cfg<br/>sudo grub-mkconfig -o /mnt/EFI/grub/grub.cfg<br/>* Note: If you got an error, try this before grub-install:<br/>sudo mount /dev/sdxx /boot/efi/<br/>sudo mount -t efivarfs efivarfs /sys/firmware/efi/efivars/

https://lbry.tv/@mlibre:e/how-to-install-grub-2-on-a-uefi-system:f