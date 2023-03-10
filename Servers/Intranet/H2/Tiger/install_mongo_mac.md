###1. 下载
```
下载tgz版本
```

&nbsp;

###2. 解压并配置环境变量
```
cd /Users/kg/install_pkg/Database
tar -zxvf mongodb-macos-x86_64-4.4.6.tgz
mv mongodb-macos-x86_64-4.4.6 /Users/kg/soft/mongodb

vi ~/.bash_profile

# mongodb
export MONGO_HOME=/Users/kg/soft/mongodb
export PATH=$PATH:$MONGO_HOME/bin

source ~/.bash_profile
```

&nbsp;

###3. 创建日志及数据存放的目录

- 数据存放路径
```
mkdir -p /Users/kg/soft/mongodb/data
mkdir -p /Users/kg/soft/mongodb/log

sudo chown kg /Users/kg/soft/mongodb/data
sudo chown kg /Users/kg/soft/mongodb/log
```

&nbsp;

###4. 启动

- 后台启动
```
mongod --dbpath /Users/kg/soft/mongodb/data --logpath /Users/kg/soft/mongodb/log/mongo.log --fork
```

- 配置文件启动
```
mongod --config /usr/local/etc/mongod.conf
```

&nbsp;

###5. 查看
```
ps aux | grep -v grep | grep mongod

cd $MONGO_HOME/bin 
./mongo
```

&nbsp;

###6. 关闭
```
cd $MONGO_HOME/bin 
./mongo

db.adminCommand({ "shutdown" : 1 })
```