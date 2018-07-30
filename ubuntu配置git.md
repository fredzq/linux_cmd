在最近的ubuntu16.04版本中，访问其他网络也正常，但最近发现git clone很慢甚至断开连接，而且无法ping github.com网站

原因：hosts文件中保存的github映射ip过期，无法解析到正确的ip地址

笔者也尝试加入域名解析无作用，也百度搜索了很多其他的办法无效，如修改 /etc/ssh/ssh_config 最后的解决办法如下

解决方法：/etc/hosts文件中将github ip地址更改为最新的正确的ip地址．

192.30.255.112  github.com git

185.31.16.184 github.global.ssl.fastly.net