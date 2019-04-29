# 配置国内源

1.  备份当前源

```bash
$ mv /etc/yum.repos.d/CentOS-Base.repo /etc/yum.repos.d/CentOS-Base.repo.bk
```

2. 下载源配置文件，或者编辑一个新的配置文件，比如下载163的源

```bash
$ wget http://mirrors.163.com/.help/CentOS7-Base-163.repo
```

3. 生成本地缓存

```bash
$ yum makecache
```

4. 更新

```bash
$ yum -y update
```

# 基础命令

获取内核版本

```bash
$ cat /proc/version
```

获取centos版本

```bash
$ cat /etc/*elease
```
