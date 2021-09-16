# config WARP

wget -N --no-check-certificate https://raw.githubusercontent.com/happy201807/YG-CFWarp-Pro/main/multi.sh && chmod +x multi.sh && ./multi.sh


# install Docker  

apt update && apt install curl

curl -fsSL https://get.docker.com | bash -s docker --mirror Aliyun

# 在Ubuntu 20.04下卸载Docker

在卸载Docker之前，最好删除所有容器、映像、卷和网络。

运行以下命令以停止所有正在运行的容器并删除所有docker对象：

docker container stop $(docker container ls -aq)

docker system prune -a --volumes

现在，可以像使用apt安装的任何其他软件包一样卸载Docker：

sudo apt purge docker-ce

sudo apt autoremove

至此，卸载Docker完成。


# run BBR plus

wget -N --no-check-certificate "https://raw.githubusercontent.com/ylx2016/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh

# aria2

wget -N --no-check-certificate https://raw.githubusercontent.com/happy201807/v2/main/aria2_install.sh && chmod +x aria2_install.sh && bash aria2_install.sh 


# WEB http server

cd /..

curl -fsSL https://raw.githubusercontent.com/smgoller/rangehttpserver/master/RangeHTTPServer.py | python

bt.cn

wget -O install.sh http://download.bt.cn/install/install-ubuntu_6.0.sh && bash install.sh

# iptables

wget https://raw.githubusercontent.com/happy201807/v2/main/iptables.sh && bash iptables.sh

# function configure_web() {

  wget -O web.tar.gz https://github.com/jiuqi9997/xray-yes/raw/main/web.tar.gz
  
    tar xzf web.tar.gz -C /www/xray_web
  
  judge "站点伪装" "web_camouflage"
  
  rm -f web.tar.gz
  
# xray start  

sudo systemctl start v2ray

sudo systemctl status v2ray
  
# oracle 开启Ubuntu 20 所有端口 #删除iptables

rm -rf /etc/iptables && reboot
