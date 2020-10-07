# Openwrt_Ubuntu_20.04_setup
Openwrt_Ubuntu_20.04_setup


```  
git clone https://github.com/openwrt/openwrt
sudo apt-get update
sudo apt-get -y install subversion g++ zlib1g-dev build-essential git \
python python3 python3-distutils libncurses5-dev gawk gettext unzip \
file libssl-dev wget libelf-dev ecj fastjar java-propose-classpath

#
sudo apt-get -y install subversion build-essential libncurses5-dev \
zlib1g-dev gawk git ccache gettext libssl-dev xsltproc zip

#
sudo apt-get -y install asciidoc binutils bzip2 gawk gettext libncurses5-dev \
libz-dev patch  zlib1g-dev lib32gcc1 libc6-dev-i386 subversion flex uglifyjs \
git-core gcc-multilib p7zip p7zip-full msmtp texinfo libglib2.0-dev xmlto \
qemu-utils upx autoconf automake libtool autopoint device-tree-compiler \
g++-multilib antlr3 gperf
#

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
  
  
the make & build is in processing,  it may take few hours to completion, depends on PC and hardware rating,

![openwrt_build_ok.JPG](openwrt_build_ok.JPG)  


  
jsut in case, if you want to delete project files, this will help,
```  
sudo rm -r openwrt
```  
