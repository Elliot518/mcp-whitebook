[Back](README.md)

<hr>

### 1. Start MongoDB

```
cd /soft/mongodb/bin
mongod --config mongodb.conf
```

&nbsp;

### 2. Check MongoDB Process

```
ps aux|grep mongo
```

&nbsp;

### 3. Shutdown MongoDB

```
cd /soft/mongodb/bin
mongo
use admin
db.shutdownServer();
```
