## Mac OSX 设置

请确保之前的Shadowsocks客户端已经彻底停止服务并且关闭,不会跟随操作系统重启而自动启动,否则会导致端口冲突.

## 操作步骤

1. [浏览器设置](Brower_settings.md),此操作为必须.如已设置请跳过
2. 安装 [V2RayX](https://github.com/Cenmrev/V2RayX/releases)
3.  Configure...
 - Local Socks5 Port: 1080
 - Support UDP: 勾选
 - Local Http Port: 8001 (http proxy port)
 - DNS: 8.8.8.8,8.8.4.4,localhost
4. Configure... -> transport settings... -> Mux
 - Enable: 勾选
 - concurrency: 8

步骤3,4为通用设置.选中所有的服务器对这些参数做设置

### 套餐一设置
1. V2ray Server 下面 +号 添加一个服务器,所需要的信息请从邮件中获取
2. Network: tcp
3. V2ray 图标上右键 -> Start V2Ray

### 套餐二设置
1. 套餐二包含套餐一内容,所以会有2个服务器,只是服务器参数有所不同,请根据套餐一的操作,创建2个服务器
2. 选中kcp的服务器:
 - Network: kcp
 - transport settings... -> Core:Kcp设置 所需要的信息请从邮件中获取,

V2ray 图标上右键 -> 服务器 选择不同的服务器即可

## 相关开源项目

 - [V2RayX](https://github.com/Cenmrev/V2RayX)

[返回主页](README.md)
