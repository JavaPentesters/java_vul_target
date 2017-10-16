# WebGoat

WebGoat是由OWASP维护包含web应用漏洞的渗透测试平台，旨在教授web应用程序安全课程

## 环境搭建

搭建及运行漏洞环境：

```
docker build -t webgoat/webgoat-8.0 . --rm=true
docker images webgoat/webgoat-8.0
docker run  -p 8080:8080 imageId前4位
```

## 漏洞说明

WebGoat包含以下几种主要的漏洞

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
