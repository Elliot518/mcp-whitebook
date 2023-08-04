### 1. Start Redis
```
redis-server /etc/redis.conf &

# 关闭firewalld防火墙，关闭开机自启
systemctl stop firewalld.service
systemctl disable firewalld.service
```

&nbsp;

### 2. Shutdown Redis
```
redis-cli shutdown
```