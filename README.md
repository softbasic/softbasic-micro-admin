# softbasic-micro-admin
对softbasic-micro-core项目的运维工具

项目名为softbasic-micro-admin，研发对微服务项目的运维、管理工具，命令以softbasic-micro命名，而不是带着admin，为的是简化日常管理的命令复杂度。

兼容Ubuntu16.04及以上版本

## 安装方法

#### On Ubuntu16.04+
```shell
curl -L http://download.softbasic.org/softbasic-micro-admin/latest/softbasic-micro >/tmp/softbasic-micro && chmod +x /tmp/softbasic-micro && cp /tmp/softbasic-micro /usr/local/bin/softbasic-micro
```

## 使用方法

##### 下载示例配置文件
````shell
curl http://download.softbasic.org/softbasic-micro-admin/latest/example.yml >/opt/project/example/example.yml
````


##### 部署，更新代码重新打包，重启项目
````shell
softbasic-micro deploy example.yml
````

##### 启动项目
````shell
softbasic-micro start example.yml
````

##### 重启项目
````shell
softbasic-micro restart example.yml
````

##### 停止项目
````shell
softbasic-micro stop example.yml
````


## 项目配置参数
```asp
1、项目名:projectName，可空
2、GIT远程仓库地址:remoteUrl，必填
```
