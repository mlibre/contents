# Advance Tips to Increase Linux Mint Speed 2019
<a href="https://www.youtube.com/watch?v=X5OOXvSgSiU">
<p align="center">
<img src="http://img.youtube.com/vi/X5OOXvSgSiU/0.jpg" alt="Advance Tips to Increase Linux Mint Speed 2019">
</p></a>


Speed Up Linux with advanced tips.  
Commands:  
````  
sudo nano /etc/sysctl.conf  
# vm.swappiness=10  
sudo nano /etc/default/grub  
# GRUB_CMDLINE_LINUX_DEFAULT="quiet splash profile"  
sudo update-grub2  
sudo apt-get purge rsyslog  
sudo nano /etc/systemd/journald.conf  
ReadKMsg=no  
# .....  
sudo nano /etc/modprobe.d/nowatchdog.conf  
# blacklist iTCO_wdt  
````  
References:

https://lbry.tv/@mlibre:e/advance-tips-to-increase-linux-mint:9

My ETH Address:
> 0xc9b64496986E7b6D4A68fDF69eF132A35e91838e