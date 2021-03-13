# How to enable and prioritize AMDGPU over radeon driver in Ubuntu, Linuxmint or Debian

[![How to enable and prioritize AMDGPU over radeon driver in Ubuntu, Linuxmint or Debian](http://img.youtube.com/vi/Mr_UFL5ZeKQ/0.jpg)](https://www.youtube.com/watch?v=Mr_UFL5ZeKQ "How to enable and prioritize AMDGPU over radeon driver in Ubuntu, Linuxmint or Debian")


How to enable and prioritize AMDGPU over Radeon driver in Ubuntu and LinuxMint.<br/>	Commands:<br/>	sudo nano /etc/default/grub<br/>	# radeon.cik_support=0 amdgpu.cik_support=1 radeon.si_support=0 amdgpu.si_support=1<br/>	sudo nano /etc/modprobe.d/amdgpu.conf<br/>	# options amdgpu si_support=1<br/>	# options amdgpu cik_support=1<br/>	sudo nano /etc/modprobe.d/radeon.conf<br/>	# options radeon si_support=0<br/>	# options radeon cik_support=0<br/>	sudo update-grub2<br/>	# If system/Linux didn't come up, Just edit the grub in the startup by pressing E, and delete the added part, and press CTRL + X to start with edited grub.

https://lbry.tv/@mlibre:e/how-to-enable-and-prioritize-amdgpu-over:2

ETH Address:
> 0xc9b64496986E7b6D4A68fDF69eF132A35e91838e