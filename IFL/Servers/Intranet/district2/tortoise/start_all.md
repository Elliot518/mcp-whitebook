### 1. Start Nacos2
```
cd /soft/nacos/bin
sh startup.sh -m standalone
# 关闭firewalld防火墙，关闭开机自启
systemctl stop firewalld.service
systemctl disable firewalld.service

# check
tail /soft/nacos/logs/start.out
http://192.168.1.100:8848/nacos
```

&nbsp;


### 2. Shutdown Nacos2
```
cd /soft/nacos/bin
sh shutdown.sh
```
