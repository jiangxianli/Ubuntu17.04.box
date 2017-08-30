# Ubuntu17.04.box
基于Ubuntu官方发布的Ubuntu17.04系统，自己安装配置一些开发使用的常用软件，而使用Vagrant定制打包的Ubuntu17.04系统。

## Box 下载地址
- 包含 Ubuntu17.04.box、Vagrant1.9.6、VirtualBox5.1.22
- 百度云盘 链接: [http://pan.baidu.com/s/1skXgbCD](http://pan.baidu.com/s/1skXgbCD) 密码: 9gt6

## 源更换

- Ubuntu 更换成 [阿里镜像源](http://wiki.ubuntu.org.cn/%E6%A8%A1%E6%9D%BF:17.04source)
- Npm 更换成  [淘宝镜像源](http://npm.taobao.org/)
- Composer 更换成 [中国镜像](https://pkg.phpcomposer.com/)

## 软件列表
- nginx / 1.10.3
- php  / 7.0.22
- mysql / 5.7.19
- npm / 3.5.2
- node / 4.2.6
- cnpm / 5.1.1
- composer / 1.5.1
- redis / 3.0.6
- mongodb / 2.6.10
- rabbitmq / 3.5.7

## 初始密码
- 系统用户 vagrant/vagrant 、root/vagrant
- Mysql用户 root/root

## 使用
```shell
    vagrant box add ubuntu17 ubuntu17.04.box
    vagrant init ubuntu17
    vagrant up ubuntu17
```

## 注意
- 如在vagrant up 连接不上ssh时，在Vagrantfile文件中配置如下代码 ，使用账号密码形式登录。
```
     config.ssh.username = "vagrant"
     config.ssh.password = "vagrant"
```
- 使用Vagrant 中你可能遇到的一些问题，请看[这里](https://www.jiangxianli.com/?tag=vagrant)
- 本项目仅供个人使用，请勿用于商业用途。
- 本Box基于官方镜像个人定制，无毒无后门，可放心使用。
- 喜欢就点个赞吧!