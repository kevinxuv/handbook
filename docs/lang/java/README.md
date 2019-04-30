# Java

## 安装

### ubuntu

参考 [digitaocean](https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-get-on-ubuntu-16-04)
```
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
```
配置Java环境:
1. 修改`/etc/enviroment` 文件加入 `JAVA_HOME="/usr/lib/jvm/java-8-oracle"`
2. 执行source /etc/environment，使其立即生效

验证：
执行`java`，如果输出的是java命令的帮助，说明安装成功。
