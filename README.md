# Lavalink

这是一个用于 Lavalink 服务器的同时运行代理和游戏的项目，支持多种协议的代理，自动构键jar执行文件。

### **使用说明**

1：fork本项目

2：在Actions菜单允许 `I understand my workflows, go ahead and enable them` 按钮

3: 击下方文件名直达文件
- [Launcher.kt](./LavalinkServer/src/main/java/lavalink/server/Launcher.kt)

4: 修改Launcher.kt文件里 132至152 行中添加需要的环境变量，不需要的留空，保存后Actions会自动构建

5: 等待5分钟后,进入actions菜单，打开运行的工作流，拉到最面下载Lavalink.jar得到Lavalink.jar.gz压缩包，解压后得到Lavalink.jar上传到容器的根目录运行即可


### **相关环境变量说明**
```
UUID=fe7431cb-ab1b-4205-a14c-d056f821b383  # 默认UUID
FILE_PATH=./logs                          # 文件路径
NEZHA_SERVER                              # Nezha服务器地址, v1: nezha.xxx.com:8008  v0: nezha.xxx.com
NEZHA_PORT                                # Nezha agent端口,v1请留空，仅v0填写
NEZHA_KEY                                 # Nezha agent密钥,面板后台安装命令里获取
ARGO_PORT                                 # Argo隧道端口
ARGO_DOMAIN                               # Argo固定隧道域名
ARGO_AUTH                                 # Argo固定隧道密钥
S5_PORT                                   # Socks5端口
HY2_PORT                                  # HY2端口
TUIC_PORT                                 # TUIC端口
ANYTLS_PORT                               # AnyTLS端口
REALITY_PORT                              # Reality端口
ANYREALITY_PORT                           # AnyReality端口
CFIP=spring.io                            # 优选域名或优选IP
CFPORT=443                                # 优选域名或优选ip对应的端口
UPLOAD_URL                                # 节点自动上传URL
CHAT_ID                                   # Telegram Chat ID
BOT_TOKEN                                 # Telegram Bot Token
NAME                                      # 节点名称
DISABLE_ARGO=false                        # 是否禁用Argo,false开启,true禁用,默认开启
