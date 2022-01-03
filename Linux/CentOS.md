### CentOS

查看centOs版本

```bash
cat /etc/redhat-release
```


```bash
uname -a #查看linux内核版本
```
#### GIT
```bash
yum install git #install git

git config --global user.name "XXX" #设置用户名
git config --global user.email xxx@xx.com

git config --list #查看git的配置

```

#### ssh记住当前机器认证

```bash
ssh-keygen #本地客户端生成
cd ~/.ssh  #查看生成的密钥

ssh-copy-id -i ~/.ssh/id_rsa.pub root@serverIp
cd ~/.ssh
vim authorized_keys

ssh root@192.168.235.22 # 检验是否生效

```

#### NPM包管理
1. 安装npm
```bash
cd /usr/local/src/
wget http://nodejs.org/dist/v0.10.24/node-v0.10.24.tar.gz

#解压源码
tar zxvf node-v0.10.24.tar.gz

#编译安装

#/usr/bin/env: ‘python’: No such file or directory解决
yum install python2
```

2. 直接安装
```bash
yum install nodejs

node --version  #view node versions

```

3. 更换源   
首先测试下阿里云上面的下载npm包的速度，使用 ` npm install ` 尝试安装。

4. 服务器3000端口无法访问



#### 本机的域名配置
windows通过修改

macOS打开文件
command+shift+G 查找/etc/hosts


#### 搭建docker环境 k8s


#### 搭建流水线 

