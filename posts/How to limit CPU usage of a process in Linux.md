# How to limit CPU usage of a process in Linux
<a href="https://youtu.be/RWHSycGXYMQ">
<p align="center">
<img src="http://img.youtube.com/vi/RWHSycGXYMQ/0.jpg" alt="How to limit CPU usage of a process in Linux">
</p></a>


How to limit CPU usage of a process in Linux using cpulimit.  
Commands:  
````  
sudo apt-get install cpulimit  
cpulimit -f -l 30 -- ffmpeg -i sample.webm sample.mkv -y  
htop  
man cpulimit  
````  
References:

https://lbry.tv/@mlibre:e/how-to-limit-cpu-usage-of-a-process-in:b

My ETH Address:
> 0xc9b64496986E7b6D4A68fDF69eF132A35e91838e