# vi-mining
On video analytic, data mining and machine learning

#Activate
vagrant up

#to enter vagrant 
vagrant ssh

## discovered and decided vagrant is not suitable for the application

#installing KWiver in ubuntu 16
sudo apt-get install git zlib1g-dev libcurl4-openssl-dev libexpat1-dev dh-autoreconf liblapack-dev libxt-dev
sudo apt-get build-dep libboost-all-dev qt5-default
sudo apt install cmake
sudo apt install git
sudo apt-get install libblas-dev liblapack-dev
sud apt install libeigen3-dev

#install fletch
mkdir fletch
cd fletch
git clone https://github.com/kitware/fletch.git
mkdir build
cd build
cmake -Dfletch_ENABLE_ALL_PACKAGES:bool=on ../fletch

#install kwiver
mkdir kwiver
cd kwiver
git clone https://github.com/kitware/kwiver.git
mkdir build
cd build
cmake -Dfletch_DIR:path=<fletch_build_directory> ../kwiver

