sudo apt install cmake libevdev-dev  
git clone https://github.com/freemind001/preview.git  
cd preview  
mkdir build  
cd build  
cmake ..  
make  
sudo make install  
sudo easy-switcher --configure  
sudo systemctl enable easy-switcher  
sudo systemctl start easy-switcher  

you can create a deb package using

dpkg-buildpackage --no-sign --build=binary --post-clean
