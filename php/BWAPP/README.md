
# bwapp是一个包含web应用漏洞的渗透测试平台

## 环境搭建

搭建及运行漏洞环境：

```
$ docker build -t bwapp/javavul:1.0.0 . --rm=true
$ docker images bwapp/javavul
# 交互创建一个容器, 本容器 80 端口映射到宿主机的 1112 端口上
$ docker run -d -p 1112:80 containerId前4位
```
