# How to overlay an audio file with an image file using ffmpeg and upload to youtube
<a href="https://youtu.be/oXEb8D8r0lw">
<p align="center">
<img src="http://img.youtube.com/vi/oXEb8D8r0lw/0.jpg" alt="How to overlay an audio file with an image file using ffmpeg and upload to youtube">
</p></a>


How to upload an audio file to youtube using FFmpeg in Linux.  
Adding an image file to an audio file and creating a video file.  
Commands:  
ffmpeg -loop 1 -i kid.jpg -i Tours.mp3 -c:v libx264 -strict experimental -b:a 256k -shortest out.mp4  
  References:

https://lbry.tv/@mlibre:e/how-to-overlay-an-audio-file-with-an:b

My ETH Address:
> 0xc9b64496986E7b6D4A68fDF69eF132A35e91838e