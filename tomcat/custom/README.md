# 自定义JDK Tomcat 环境

```
docker build -t custom/tomcat:7.0.73 . --rm=true
docker images custom/tomcat
docker run -it -p 1115:8080 镜像前4位
```
不需要加-d 直接进入 /bin/bash
