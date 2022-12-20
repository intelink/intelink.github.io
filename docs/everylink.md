# 介绍

更加方便的通过”跳板机“连接到被限制访问的服务，像访问本地一样简单。支持TCP、SSH、HTTP协议等。

# 使用场景

* SSH连接
* HTTP访问

# 下载

https://url36.ctfile.com/f/7718336-751518741-a29374?p=7222 (访问密码: 7222)

# 配置
软件相同目录新建config.json文件，config.json配置见下文

默认读取当前目录config.json文件，可通过`-c`指定配置文件

例如：EveryLink.exe -c abc.json

config.json配置如下：

``` json
{
  "server_addr": "跳板机服务 如：ip:port",
  "user_name": "账号",
  "password": "密码",
	
  "server_map": [
    {"loc_addr": "本地端口1 如（:6001）", "remote_addr": "目标服务1ip:port"},
	{"loc_addr": "本地端口2 如（:6002）", "remote_addr": "目标服务2ip:port"},
  ]
}
```