# Openwrt_Ubuntu_20.04_setup
Openwrt_Ubuntu_20.04_setup


```  
git clone https://github.com/openwrt/openwrt
sudo apt-get update
sudo apt-get install subversion g++ zlib1g-dev build-essential git \
python python3 python3-distutils libncurses5-dev gawk gettext unzip \
file libssl-dev wget libelf-dev ecj fastjar java-propose-classpath
sudo apt-get install subversion build-essential libncurses5-dev \
zlib1g-dev gawk git ccache gettext libssl-dev xsltproc zip
sudo update-alternatives --install /usr/bin/python python /usr/bin/python2 1  
sudo update-alternatives --install /usr/bin/python python /usr/bin/python3 2  
sudo update-alternatives --list python  
sudo update-alternatives --config python  
python -V  
cd ~/openwrt
./scripts/feeds update -a
./scripts/feeds install -a
make menuconfig
make
```  
