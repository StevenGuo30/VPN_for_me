# V2ray搭建教程，vps搭建v2ray方法，vpn搭建v2ray 一键搭建代码
V2ray搭建视频教程：▶ https://youtu.be/VSKhge6dKm8
### 步骤：<br>
**1、Vultr注册账号**：https://www.vultr.com/?ref=8753714<br>

**2、选择服务器**<br>

**3、打开搭建工具 FinalShell**<br>
FinalShell：[点击下载>>](https://kjfx.lanzoui.com/iqm6Uosbzha)<br>
备用下载（含MAC版）：<a href="http://www.hostbuf.com/t/988.html" target="_blank">点击下载>></a><br>

**4、V2Ray一键安装代码**<br>

    bash <(curl -s -L https://git.io/v2ray-setup.sh)

<br>

    #放行端口
    iptables -I INPUT -p tcp --dport 80 -j ACCEPT
    iptables -I INPUT -p tcp --dport 8080 -j ACCEPT

BBR加速

    echo "net.core.default_qdisc=fq" >> /etc/sysctl.conf
    echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.conf
    sysctl -p

**5、科学上网软件下载**<br>
软件下载：https://github.com/Kejifaxian/welcome

**PS：如果不能访问youtube、chatgpt等网站的处理方法**
检查IPV6是否正常开启
