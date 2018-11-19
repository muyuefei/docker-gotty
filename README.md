# docker-gotty 模拟终端

***

### *参考*
[github 地址](https://github.com/yudai/gotty)

### **使用步骤**
1. git clone git@github.com:muyuefei/docker-gotty.git
2. cd docker-gotty/compose
3. docker-compose up -d

### *Demo*
[http://ip_addr:port/?arg=vim)

### **配置文件**
```yaml
version: '2'
services:
  gotty:
    build:
      context: ../gotty
      args:
        - account= //gotty base auth 用户名
        - password= //gotty base auth 密码
        - command= // gotty 执行命令
    ports:
      - "8888:8888" //gotty server 端口映射
```
