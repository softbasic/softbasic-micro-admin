# softbasic-micro-admin
基于softbasic-micro-core框架项目的运维工具

项目名为softbasic-micro-admin，研发对微服务项目的运维、管理工具，命令以softbasic-micro命名，而不是带着admin，为的是简化日常管理的命令复杂度。

兼容Ubuntu16.04及以上版本

## 安装方法

#### On Ubuntu16.04+
```shell
curl -L https://download.softbasic.org/softbasic-micro-admin/latest/softbasic-micro >/tmp/softbasic-micro && chmod +x /tmp/softbasic-micro && cp /tmp/softbasic-micro /usr/local/bin/softbasic-micro
```

## 使用方法

##### 部署，更新代码重新打包
````shell
softbasic-micro deploy example.yaml
````

##### 启动项目
````shell
softbasic-micro start example.yaml
````

##### 重启项目
````shell
softbasic-micro restart example.yaml
````

##### 停止项目
````shell
softbasic-micro stop example.yaml
````


## 项目配置参数
```asp
1、项目名:projectName
2、GIT远程仓库地址:remoteUrl
3、GIT源码的本地副本地址:srcPath,默认:/opt/project/source/$projectName
4、项目安装运行的目录:projectPath,默认：/opt/project/$projectName
5、程序打包的JAR名：jarName,默认:app.jar
```
