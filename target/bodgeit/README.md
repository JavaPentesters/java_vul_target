# bodgeit是一个包含web应用漏洞的渗透测试平台

## 环境搭建

搭建及运行漏洞环境：

```
docker build -t bodgeit/javavul:1.4.0 . --rm=true
docker images bodgeit/javavul
docker run -d -p 1111:8080 containerId前4位
```

## 漏洞说明

BodgeIt Store包含以下几种主要的漏洞

1. 跨站脚本漏洞
2. SQL注入
3. Hidden (but unprotected) content
4. CSRF漏洞
5. 调试模式(Debug code)
6. 不安全对象应用(Insecure Object References)
7. 应用逻辑漏洞

### 1. 跨站脚本漏洞利用过程



### 2. SQL注入利用过程


### 3. CSRF漏洞利用过程
