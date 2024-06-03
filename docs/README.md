
sudo apt install vim ssh gcc make curl net-tools aptitude traceroute htop expect git stress ifmetric  g++ unzip -y


sudo sed -i 's/^#DefaultTimeoutStartSec=90s/DefaultTimeoutStartSec=9s/; s/^#DefaultTimeoutStopSec=90s/DefaultTimeoutStopSec=9s/' /etc/systemd/system.conf && sudo systemctl daemon-reload

sudo sed -i 's/enabled=1/enabled=0/' /etc/default/apport


 1. sudo apt install libqt5qml5 libqt5quick5 libqt5quickwidgets5 qml-module-qtquick2 libgsettings-qt1 -y
    2. sudo wget --no-check-certificate -O /root/sogoupinyin_4.2.1.145_amd64.deb  https://fs.itsz.cc/chfs/shared/ubuntu/sogoupinyin_4.2.1.145_amd64.deb  && cd /root/
    3. sudo apt install ./sogoupinyin_4.2.1.145_amd64.deb -y&& sudo apt install -f

无线驱动安装
 wget https://raw.githubusercontent.com/pimlie/ubuntu-mainline-kernel.sh/master/ubuntu-mainline-kernel.sh
sudo install ubuntu-mainline-kernel.sh /usr/local/bin/


#第一步，让我们安装一些依赖

sudo apt install flex bison make vim gcc git -y

#第二步，下载驱动文件并编译

git clone https://gitee.com/ixianhao/intel-wifi.git

sudo cp intel-wifi/fw-binaries/*.ucode /lib/firmware

cd intel-wifi/iwlwifi-stack-dev

sudo make defconfig-iwlwifi-public

sudo make

sudo make install

#第三步，下载官网驱动文件


git clone git://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware.git

cd linux-firmware/

sudo cp iwlwifi-* /lib/firmware/

#或者在官网下载固件Linux Support for Intel® Wireless Adapters ，将解压后的ucode文件复制在/lib/firmware目录。

https://www.intel.com/content/www/us/en/support/articles/000005511/wireless.html

#第四步，重启你的电脑！


wget  https://fs.itsz.cc/chfs/shared/Ubuntu/domain/test/realm.sh
wget  --no-check-certificate   https://fs.itsz.cc/chfs/shared/ubuntu/domain/realm/realm.sh
sudo usermod -aG adm,cdrom,sudo,dip,plugdev,lpadmin,sambashare

https://github.com/tomaspinho/rtl8821ce

已经安装了谷歌浏览器，飞书，搜狗输入法(ctrl+space切换)，公司vpn工具




sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

sudo apt update

sudo apt install ros-noetic-desktop-full

echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
source ~/.bashrc

sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential

sudo apt-get install python3-pip 

sudo pip3 install rosdepc

sudo rosdepc init
rosdepc update

sudo apt install python3-roslaunch

wget -qO- https://dl.winehq.org/wine-builds/winehq.key | sudo apt-key add -
sudo apt install software-properties-common
sudo apt-add-repository "deb http://dl.winehq.org/wine-builds/ubuntu/ $(lsb_release -cs) main"
sudo apt install --install-recommends winehq-stable
wget https://raw.githwin    ubusercontent.com/Winetricks/winetricks/master/src/winetricks

