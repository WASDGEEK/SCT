## 准备

    apt-get install -y git
## 安装

    cd /opt
    git clone https://github.com/WASDGEEK/SecureTunnel.git
    cd SecureTunnel

程序位置 /opt/SecureTunnel
配置文件 config.json
启动命令 systemctl start SecureTunnel
关闭命令 systemctl stop SecureTunnel
重启命令 systemctl restart SecureTunnel
查看状态/日志 systemctl status SecureTunnel -l
开机自启动命令 systemctl enable SecureTunnel
关闭开机自启动命令 systemctl disable SecureTunnel
