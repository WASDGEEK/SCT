## 准备

    apt-get install -y git
## 安装

    cd /opt
    git clone https://github.com/WASDGEEK/SecureTunnel.git
    cd SecureTunnel
## 其他
    程序位置 /opt/SecureTunnel
    配置文件 config.json
    启动命令 systemctl start SecureTunnel
    关闭命令 systemctl stop SecureTunnel
    重启命令 systemctl restart SecureTunnel
    查看状态/日志 systemctl status SecureTunnel -l
    开机自启动命令 systemctl enable SecureTunnel
    关闭开机自启动命令 systemctl disable SecureTunnel
## 禁用IPv6
    echo " ">>/etc/sysctl.conf
    echo "# made for disabled IPv6 in $(date +%F)">>/etc/sysctl.conf
    echo 'net.ipv6.conf.all.disable_ipv6 = 1'>>/etc/sysctl.conf
    echo 'net.ipv6.conf.default.disable_ipv6 = 1'>>/etc/sysctl.conf
    echo 'net.ipv6.conf.lo.disable_ipv6 = 1'>>/etc/sysctl.conf
    tail -5 /etc/sysctl.conf
    sysctl -p
    netstat -anptl
