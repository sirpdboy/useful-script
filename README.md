# useful-script
wget -N --no-check-certificate "https://raw.githubusercontent.com/sirpdboy/useful-script/master/bbr" && chmod +x bbr.sh && ./bbr
2023-0525 检测是否可以访问 ChatGPT 脚本 来源

bash <(curl -Ls https://raw.githubusercontent.com/missuo/OpenAI-Checker/main/openai.sh)
2023-4-29 修改检测是否可以访问 ChatGPT 脚本

bash <(curl -Ls https://ourl.co/oaic)

bash <(curl -Ls https://cdn.jsdelivr.net/gh/missuo/OpenAI-Checker/openai.sh)
综合工具箱（强烈推荐，集成了很多脚本）
wget -O box.sh https://raw.githubusercontent.com/BlueSkyXN/SKY-BOX/main/box.sh && chmod +x box.sh && clear && ./box.sh
杜甫测试
wget -q https://github.com/Aniverse/A/raw/i/a && bash a
DD 相关
1、甲骨文 DD 脚本
DD 成 Debian 10

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/MoeClub/Note/master/InstallNET.sh') -d 10 -v 64 -p "自定义root密码" -port "自定义ssh端口"
DD 成 Ubuntu 20.04

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/MoeClub/Note/master/InstallNET.sh') -u 20.04 -v 64 -p "自定义root密码" -port "自定义ssh端口"
2、MoeClub 脚本
重点推荐：

时间：22/11/2021 15:21 萌咖更新脚本：

1. 新增对 Oracle AMD，Oracle ARM 全面支持。可支持从 Ubuntu, Oracle Linux 等系统网络重装.
2. 更新 dd 镜像的基础系统版本.
3. 移除对外部 wget 的依赖.
4. 新增 -port 参数，可更改默认 SSH 端口.
5. 更新 内置的网络参数计算 逻辑.
6. 更新 grub 配置文件定位逻辑，可支持任意引导 grub 的系统.

以下系统已通过测试 (其他自测):
Debian: 9, 10, 11;
Ubuntu: 18.04, 20.04;
CentOS: 6.10;
以下平台已通过测试 (其他自测):
Oracle、Do、Azure

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/MoeClub/Note/master/InstallNET.sh') -d 10 -v 64 -p "自定义root密码" -port "自定义ssh端口"
-d 10 -v 64
-d 9 -v 64
-u 20.04 -v 64
-u 18.04 -v 64

开机改密码脚本：

开机改密：

#!/bin/bash
echo root:Vicer |sudo chpasswd root
sudo sed -i 's/^#\?PermitRootLogin.*/PermitRootLogin yes/g' /etc/ssh/sshd_config;
sudo sed -i 's/^#\?PasswordAuthentication.*/PasswordAuthentication yes/g' /etc/ssh/sshd_config;
sudo reboot
3、另一位大佬的脚本
wget --no-check-certificate -O AutoReinstall.sh https://git.io/AutoReinstall.sh && bash AutoReinstall.sh
CentOS 默认密码 Pwd@CentOS 其它系统 Pwd@Linux

OpenVZ / LXC 架构系统不适用

来源：https://blog.hicasper.com/post/135.html 参考：https://www.ydyno.com/archives/1245.html 感谢大佬的付出！

bash <(wget --no-check-certificate -qO- 'https://file.geekn.net/CNODnjau/InstallNET.sh') -d 11 -v 64 -a -firmware
-firmware 额外的驱动支持
-d 后面是系统版本号
-v 后面写 64 位 32 位
-a （不清楚这个干啥的但是每个脚本都带）
–mirror 后面是镜像源地址

-p 后面写自定义密码

镜像站地址
官方给出的地址列表：https://www.debian.org/mirror/list

一些国内的
ftp.cn.debian.org
mirror.bjtu.edu.cn
mirror.lzu.edu.cn        
mirror.nju.edu.cn        
mirrors.163.com        
mirrors.bfsu.edu.cn        
mirrors.hit.edu.cn        
mirrors.huaweicloud.com        
mirror.sjtu.edu.cn        
mirrors.tuna.tsinghua.edu.cn        
mirrors.ustc.edu.cn        

使用方法：（大致都是一样的）

清华源
--mirror 'https://mirrors.ustc.edu.cn/debian/'

腾讯源
--mirror 'https://mirrors.aliyun.com/debian/'

阿里源
--mirror 'https://mirrors.aliyun.com/debian/'

华为源
--mirror 'https://mirrors.huaweicloud.com/debian/'
4、秋水逸冰 Windows 2012/2016/2019/2022 10/11 DD 镜像
适用于 UEFI 启动的多个 Windows 系统 DD 镜像：

https://teddysun.com/656.html

分别是：

Windows Server 2012 R2 Datacenter
Windows Server 2016 Datacenter (build: 14393.5006)
Windows Server 2019 Datacenter (build: 17763.2686)
Windows Server 2022 Datacenter (build: 20348.587)
Windows 10 Enterprise LTSC (build: 19044.1288)
Windows 11 Pro for Workstations 21H2 (build: 22000.194)
适用于 BIOS 启动的 Windows Server 2022 Datacenter DD 镜像：

https://teddysun.com/629.html

适用于 BIOS 启动的 Windows 11 Pro for Workstations 21H2 DD 镜像：

https://teddysun.com/642.html

适用于 BIOS 启动的 Windows 10 Enterprise LTSC DD 镜像：

https://teddysun.com/640.html

适用于 BIOS 启动的 Windows Server 2019/2016/2012R2 Datacenter DD 镜像：

https://teddysun.com/545.html

分别是：

Windows Server 2019 Datacenter（Build: 17763.2686）
Windows Server 2016 Datacenter（Build: 14393.5006）
Windows Server 2012 R2 Datacenter
测试相关
机器测试
单线程测试
bash <(curl -Lso- https://bench.im/hyperspeed)
最全测速脚本
curl -fsL https://ilemonra.in/LemonBenchIntl | bash -s fast
superbench
wget -qO- git.io/superbench.sh | bash
Bench.sh
wget -qO- bench.sh | bash
速度测试
显示延迟、抖动
bash <(wget -qO- https://bench.im/hyperspeed)
直接显示回程线路
curl https://raw.githubusercontent.com/zhucaidan/mtr_trace/main/mtr_trace.sh|bash
wget -q route.f2k.pub -O route && bash route
# 第一个
wget https://raw.githubusercontent.com/nanqinlang-script/testrace/master/testrace.sh
bash testrace.sh

# 第二个
wget -qO- git.io/besttrace | bash
四网测速
wget -O jcnf.sh https://raw.githubusercontent.com/Netflixxp/jcnfbesttrace/main/jcnf.sh

bash jcnf.sh
三网测速
bash <(curl -Lso- https://git.io/superspeed_uxh)
带快速四网测试版本：

bash <(curl -Lso- https://dl.233.mba/d/sh/speedtest.sh)
bash <(curl -Lso- https://git.io/J1SEh)
测试 25 端口是否开放
telnet smtp.aol.com 25
测试 IPv4 优先还是 IPv6 优先
复制成功
curl ip.p3terx.com
流媒体测试
全媒体测试
bash <(curl -L -s https://raw.githubusercontent.com/lmc999/RegionRestrictionCheck/main/check.sh)
奈飞测试
wget -O nf https://github.com/sjlleo/netflix-verify/releases/download/2.5/nf_2.5_linux_amd64 && chmod +x nf && clear && ./nf
#第一个
bash <(curl -L -s https://raw.githubusercontent.com/lmc999/RegionRestrictionCheck/main/check.sh)

# 第二个
bash <(curl -sSL "https://github.com/CoiaPrant/MediaUnlock_Test/raw/main/check.sh")
WARP
wget -N --no-check-certificate https://cdn.jsdelivr.net/gh/YG-tsj/CFWarp-Pro/multi.sh && chmod +x multi.sh && ./multi.sh
之后进入脚本快捷方式为 bash multi.sh

服务器时间
CentOS 同步时间
复制成功
yum -y install ntpdate
timedatectl set-timezone Asia/Shanghai
ntpdate ntp1.aliyun.com
BBR
CentOS 7 BBR
复制成功
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
一键开启 BBR
注意：需要 Linux Kernel 内核升级到 4.9 及以上版本可以实现 BBR 加速

uname -srm
输出结果：

Linux 3.10.0-957.12.2.el7.x86_64 x86_64
3 - 内核版本.
10 - 主修订版本.
0-957 - 次要修订版本.
12 - 补丁版本.
一般来说，Ubuntu18.04 以上就可以 (默认的内核 4.15)

echo "net.core.default_qdisc=fq" >> /etc/sysctl.conf
echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.conf

sysctl -p

sysctl net.ipv4.tcp_available_congestion_control

lsmod | grep bbr
Docker 相关
更新、安装必备软件
apt-get update && apt-get install -y wget vim
海外服务器
非大陆 Docker 安装
wget -qO- get.docker.com | bash
卸载 Docker
sudo apt-get purge docker-ce docker-ce-cli containerd.io
sudo rm -rf /var/lib/docker
sudo rm -rf /var/lib/containerd
非大陆 Docker-compose 安装
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
查看版本

docker-compose --version
大陆服务器
国内机安装 docker
curl -sSL https://get.daocloud.io/docker | sh
国内机安装 docker-compose
curl -L https://get.daocloud.io/docker/compose/releases/download/v2.1.1/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
卸载 docker
sudo apt-get remove docker docker-engine
rm -fr /var/lib/docker/
防火墙
CentOS 关闭防火墙
systemctl start supervisord
systemctl disable firewalld
systemctl stop firewalld
宝塔相关
宝塔去除登陆 (已经失效，解决方法见：https://blog.laoda.de/archives/bt-to-aapanel)
sed -i "s|if (bind_user == 'True') {|if (bind_user == 'REMOVED') {|g" /www/server/panel/BTPanel/static/js/index.js
rm -rf /www/server/panel/data/bind.pl
宝塔 & aapanel 破解（这个目前也不保证可用了）
# 宝塔&aapanel破解
编辑 /www/server/panel/class/panelplugin.py
找到 softList['list'] = tmpList 这行代码
在下面添加以下代码，注意缩进

softList['pro'] = 1
for soft in softList['list']:
soft['endtime'] = 0

编辑完毕后保存重启面板即可
呆梨相关
XUI
bash <(curl -Ls https://raw.githubusercontent.com/FranzKafkaYu/x-ui/master/install.sh)
脚本来源：https://github.com/FranzKafkaYu/x-ui

mack-a
wget -P /root -N --no-check-certificate "https://raw.githubusercontent.com/mack-a/v2ray-agent/master/install.sh" && chmod 700 /root/install.sh && /root/install.sh
持续更新中
