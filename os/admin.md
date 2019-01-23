# 系统管理员

## systemd
systemd是用来管理Linux系统服务的一款程序，提供服务的初始化、启动、关闭等功能，目前主要的Linux系统都已经把systemd作为默认的init system

### 使用
不同的Linux系统都有自己的包的管理工具，通过这些工具可以安装你需要安装的应用程序，基本上大部分流行的应用程序都会支持大部分的Linux系统，他们在打包的时候会针对不同的Linux系统打包出不同的package安装包，然后上传到他们的包的仓库里面，当通过包管理工具安装命令安装完应用程序的时候，大部分的应用程序都会生成systemd的unit配置文件，这时候你还需要执行下面命令用来enable:
```
$ systemctl enable *.service # *.service代表的是你的应用程序的systemd unit file name，或者是service name，你可以从systemd存放unit file的目录找到，比如nginx的名称就是nginx.service
```
systemctl是systemd的命令行工具，用来执行systemd的功能，有些程序可能在安装后就启动了，所以就可以不用enable，这时候你可以运行下面命令检测出是否已经启动：
```
$ systemctl status *.service
```
你可以看到如果有类似的服务已经启动的输出，说明本身服务已经启动，如果没有可以执行下面的命令启动服务:
```
$ systemctl start *.service
```
还有常用的命令如下：
```
$ systemctl restart *.service # 重启服务
$ systemctl stop *.service # 停止服务
```
这样借助systemd你可以很好的管理你安装的应用程序

### references
[官方文档](https://www.freedesktop.org/wiki/Software/systemd/)

[wikipedia](https://en.wikipedia.org/wiki/Systemd)

[digitalocean](https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units)
