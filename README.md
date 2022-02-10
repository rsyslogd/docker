## 收集并验证的常用服务Docker Compose脚本

基于CentOS7，Docker Version: 20.10.11，docker-compose version 1.29.2

- 本脚本将持续更新

前提建议：

1. CentOS7系统的VPS并已初始化
2. 安装了docker-ce-20.10.11和docker-compose version 1.29.2
3. 防火墙策略（iptables和服务器管理中安全组）允许所有来源的访问

## 运行步骤

1. checkout本项目，进入需要的服务，有.env文件则根据需要修改它
2. 运行`docker-compose up -d`, 启动相关服务

> 注意：
> .env 预设的密码建议修改


## 服务端脚本简介

Docker Compose启动服务：

```bash
docker-compose up -d
```

在当前目录下查看日志

```bash
docker-compose logs -f
```

查看已经启动的容器

```
docker ps
```

