Title: 在CentOS中安装并配置 Redis
Published: 2019-09-23
Tags: ["Redis","CentOS","Linux"]
---
#### 1.下载Redis
```
wget http://download.redis.io/releases/redis-5.0.5.tar.gz
```

#### 2. 解压安装包
```
tar -zxvf redis-5.0.5.tar.gz
```

#### 3. 在 解压出来的目录中，执行 make 命令编译
```
cd redis-5.0.5
make
```

#### 4. 运行 make test, 进行测试
#### 5. 安装
```
# 安装到默认目录 /usr/local/bin/
make install 
# 安装到指定目录
make install PREFIX=/root/my_apps/redis

# copy 配置文件到指定的目录
cp redis-5.0.5/redis.conf ./redis
```

#### 6. 修改配置文件
把daemonize no 改成 daemonize yes
> 表示后台运行

bind:
```
bind 127.0.0.1 192.168.1.13
#bind 127.0.0.1 192.168.1.13
注释掉之后，会允许所有的连接到redis server
```
protected-mode no
> 默认时yes， 当设置成no的时候，不会要求验证，完全开放



#### 7. 常用命令
启动：
```
./bin/redis-server redis.conf
```
连接到redis的命令
```

停止:
```
./bin/redis-cli showdown
```

# 连接到本机的redis 服务
./bin/redis-cli 

# 连接到指定的远程服务
./redis-cli -h 127.0.0.1 -p 6379
```
#### 8. 其他命令说明
- Redis-server 启动服务
- Redis-cli 访问到redis的控制台
- redis-benchmark 性能测试的工具
- redis-check-aof aof文件进行检测的工具
- redis-check-dump  rdb文件检查工具
- redis-sentinel  sentinel 服务器配置



