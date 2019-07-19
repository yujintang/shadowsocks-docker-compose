# shadowsocks-docker-compose
快速部署VPN

## 安装环境
- 安装 Docker、docker-compose

## 使用项目列表
* redis: https://github.com/antirez/redis
* shadowsocks-python: https://github.com/shadowsocks/shadowsocks
* shadowsocks-manager: https://github.com/shadowsocks/shadowsocks-manager

## 下载项目
```
git clone git clone https://github.com/yujintang/shadowsocks-docker-compose.git
cd shadowsocks-docker-compose
```
## 修改shadowsocks配置
1. 修改服务器的IP地址  .ssmgr/webgui.yml

![](https://raw.githubusercontent.com/yujintang/imageHosting/master/wechat/WechatIMG5816.jpeg)

2. 修改邮箱配置(注册用户发送注册码，修改密码等操作) .ssmgr/webgui.yml 
![](https://raw.githubusercontent.com/yujintang/imageHosting/master/wechat/WeChat8958daa430434ee93d2dd60aaaa003e0.png)

3. 修改管理员用户名、密码（初始用户用来管理web admin） .ssmgr/webghui.yml
![](https://raw.githubusercontent.com/yujintang/imageHosting/master/wechat/WeChatbcddc8b9533ed431ead0d73a11cfedae.png)

## 启动项目
```
docker-compose up -d --build
```
## 登陆web端
> 10000 端口如需修改，需要修改.ssmgr/webgui.yml webgui.port部分，然后修改docker-compose.yml shadowsocks-manager.ports 部分, 然后登陆
```
http://ip:10000
```
## 添加账号、感受外面的世界吧

## 客户端推荐
* android: https://github.com/shadowsocks/shadowsocks-android/releases/download/v4.7.4/shadowsocks--universal-4.7.4.apk
* mac: https://github.com/shadowsocks/ShadowsocksX-NG/releases/download/v1.8.2/ShadowsocksX-NG.app.1.8.2.zip
* windows: https://github.com/shadowsocks/shadowsocks-windows/releases/download/4.1.7.1/Shadowsocks-4.1.7.1.zip

## 其他
### 服务器端口：
部署服务器上，需要开启10000、4001、55000-55099 端口，如需更多用户账号，需要扩大端口范围，请自行调整
### 常用邮件服务器

| 邮箱服务商 | pop3 | smtp |
| --  |  --- | -- |
| gmail.com: | :pop.gmail.com | :smtp.gmail.com|
| 21cn.com:  | :pop.21cn.com  | :smtp.21cn.com|
| sina.com:  | :pop3.sina.com.cn  | :smtp.sina.com.cn |
| tom.com:  | :pop.tom.com  | :smtp.tom.com |
| 163.com:  | :pop.163.com  | :smtp.163.com |
| 263.net:  | :pop3.263.net  | :smtp.263.net |
| x263.net:  | :pop.x263.net  | :smtp.x263.net |
| 263.net.cn:  | :pop.263.net.cn  | :smtp.263.net.cn |
| elong.com:  | :pop3.elong.com  | :smtp.elong.com |
| china.com:  | :pop.china.com  | :smtp.china.com |
| sohu.com:  | :pop3.sohu.com  | :smtp.sohu.com |
| etang.com:  | :pop.etang.com  | :smtp.etang.com |
| yahoo.com:  | :pop.mail.yahoo.com  | :smtp.mail.yahoo.com |
| yahoo.com.cn:  | :pop.mail.yahoo.com.cn  | :smtp.mail.yahoo.com.cn |

### shadowsocks-manager 官方配置文档
> https://shadowsocks.github.io/shadowsocks-manager/#/home

