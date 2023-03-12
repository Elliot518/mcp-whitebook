[Back](README.md)

<hr>

### 1. Start MySQL
```
cd /usr/local/mysql

./support-files/mysql.server start

systemctl stop firewalld.service
systemctl disable firewalld.service
```

&nbsp;

### 2. Stop MySQL
```
cd /usr/local/mysql

./support-files/mysql.server stop
```



