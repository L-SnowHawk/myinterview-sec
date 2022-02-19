# Sec-Interview-Personal

## 0x00 校招-2022-安服

1. SQL注入漏洞原理、防御

2. 应急响应流程-挖矿木马

   1. 爆破登录ssh看什么日志文件）
      1. /var/log/secure

   2. 溯源关键点是什么因素
   3. atime mtime ctime分别是什么）
      1. Access访问时间 Modify修改时间 Change状态改变时间 可以stat * 查看这个目录所有文件的状态
      2. mtime 文件内容修改时间，而不是文件属性的修改，当数据内容修改时，这个时间就会改变，命令ls -l默认显示的就是这个时间
      3. ctime 状态时间，当一个文件的状态改变时，这个时间就会改变，例如更改了文件的权限与属性等，它就会改变
      4. atime 访问时间，当读取文件内容时，就会更改这个时间，例如使用cat /etc/config 那么该文件的atime就会改变
   4. 如何查看监听端口服务等）
      1. netstat -tunlp 各个参数作用

3. 文件上传有哪些绕过

4. Burp如何修改返回包 Response

5. SQLMAP -参数 --参数有什么区别 如何指定位置测试诸如点

6. XSS漏洞原理、防御

7. CSRF/SSRF是什么，区别在哪里，SSRF能干什么

8. 内网信息收集

9. 拿到一台工作组机器权限，但是不在域内的情况下如何定位域控

10. 了解Webshell吗，有没有尝试写过，内存马是什么

