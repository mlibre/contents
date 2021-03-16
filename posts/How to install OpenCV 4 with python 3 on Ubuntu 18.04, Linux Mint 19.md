# How to install OpenCV 4 with python 3 on Ubuntu 18.04, Linux Mint 19
<a href="https://youtu.be/FDjsLK9M6Sc">
<p align="center">
<img src="http://img.youtube.com/vi/FDjsLK9M6Sc/0.jpg" alt="How to install OpenCV 4 with python 3 on Ubuntu 18.04, Linux Mint 19">
</p></a>


Install OpenCV 4 with Python 3 on Ubuntu 18.04, Linux Mint 19.  
Commands:  
````  
mkdir ~/opencv_install  
cd opencv_install  
sudo apt-get update   
sudo apt-get dist-upgrade  
sudo apt purge libx264-dev x264  
sudo apt-get install build-essential cmake pkg-config libjpeg8-dev libtiff5-dev libpng12-0  
sudo apt install v4l-utils libv4l-dev libgphoto2-dev libgstreamer1.0-0 libgstreamer1.0-dev x264  
cd /usr/include/linux/  
sudo ln -s -f ../libv4l1-videodev.h videodev.h  
cd ~/opencv_install  
sudo apt install libavcodec-dev libavformat-dev libswscale-dev libxvidcore-dev   
sudo apt install libgtk-3-dev libatlas-base-dev gfortran python3.6-dev python2.7-dev libtiff-dev  
@ install pip  
aria2c "https://bootstrap.pypa.io/get-pip.py"  
sudo python3 get-pip.py  
sudo pip install numpy  
sudo pip3 install numpy  
aria2c "https://github.com/opencv/opencv/archive/4.0.1.zip"  
aria2c "https://github.com/opencv/opencv_contrib/archive/4.0.1.tar.gz"  
tar xvf opencv_contrib-4.0.1.tar.gz  
mkdir opencv  
cd opencv/  
cp ../opencv-4.0.1.zip .  
unzip opencv-4.0.1.zip  
cd opencv-4.0.1/  
mkdir build  
cd build  
cmake -D CMAKE_BUILD_TYPE=RELEASE -D WITH_V4L=ON -D CMAKE_INSTALL_PREFIX=/usr/local -D INSTALL_PYTHON_EXAMPLES=ON  -D INSTALL_C_EXAMPLES=OFF -D PYTHON_EXECUTABLE=/usr/bin/python3.6  -D BUILD_EXAMPLES=ON -D OPENCV_EXTRA_MODULES_PATH=../../../opencv_contrib-4.0.1/modules ..  
make -j4  
make  
sudo make install  
sudo ldconfig  
python3.6  
import cv2  
cv2.__version__  
````References:

https://lbry.tv/@mlibre:e/how-to-install-opencv-4-with-python-3-on:2

My ETH Address:
> 0xc9b64496986E7b6D4A68fDF69eF132A35e91838e