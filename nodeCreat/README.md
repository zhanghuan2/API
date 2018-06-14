## init host

进入服务端

### code
```
  ssh root@172.16.101.154
```


=====================================================================================

## download nodejs


### 构建方式
```
  sudo uname --m   // show linx config
  wget https://nodejs.org/dist/v8.11.1/node-v8.11.1-linux-x64.tar.xz
  //download nodeJs 8.11.1

  tar -xvf node-v8.11.1-linux-x64.tar.xz  //解压缩

  //设置全局环境变量
  ln -s /usr/local/src/node-v8.11.1-linux-x64/bin/node /usr/local/bin/node

  ln -s /usr/local/src/node-v8.11.1-linux-x64/bin/npm /usr/local/bin/npm
  node -v
  npm -v

```


