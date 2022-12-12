
## 安装脚本

- 输入【**vasma**】管理脚本，脚本执行路径[**/etc/v2ray-agent/install.sh**]


```
wget -P /root -N --no-check-certificate "https://raw.githubusercontent.com/ttagxwr/v2rayn/master/install.sh" && chmod 700 /root/install.sh && /root/install.sh
```
———————————————————————————————————————————————————————————————

Debian8启动nginx失败

解决方法一

手动删除add_header选项

vim /etc/nginx/conf.d/alone.conf

# 删除下方代码

add_header Strict-Transport-Security "max-age=63072000" always;

——————————————————————————————

4.低版本升级高版本后无法启动核心

1.先分别执行下方命令

2.使用脚本中[13.core管理]启动即可

systemctl stop trojan-go

systemctl disable trojan-go

————————————


脚本目录

—————


Xray-core

主目录

/etc/v2ray-agent/xray


配置文件目录

/etc/v2ray-agent/xray/conf


————————————

v2ray-core

主目录

/etc/v2ray-agent/v2ray


配置文件目录

/etc/v2ray-agent/v2ray/conf

————————————

Trojan

目录

/etc/v2ray-agent/trojan

————————————


TLS证书

目录

/etc/v2ray-agent/tls

————————————

Nginx

Nginx配置文件

/etc/nginx/conf.d/alone.conf

————————————


Nginx伪装站点目录

/usr/share/nginx/html

————————————
