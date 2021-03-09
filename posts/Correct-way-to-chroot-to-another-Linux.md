# Correct way to chroot to another Linux

[![Correct way to chroot to another Linux](http://img.youtube.com/vi/l0wpWUyUSuI/0.jpg)](https://www.youtube.com/watch?v=l0wpWUyUSuI "Correct way to chroot to another Linux")


Properly prepare a Linux system for chroot to another one.<br/>Commands:<br/>sudo mount /dev/sdb1 /mnt/<br/>sudo mount -t proc none /mnt/proc<br/>sudo mount --bind /sys /mnt/sys<br/>sudo mount --bind /dev /mnt/dev<br/>sudo chroot /mnt

https://lbry.tv/@mlibre:e/correct-way-to-chroot-to-another-linux:6