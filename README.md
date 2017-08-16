# Ubuntu16.04.box
基于Vagrant.box 官方发布的Ubuntu16.04系统，自己安装配置一些开发使用的常用软件，而定制打包的Ubuntu16.04系统。

## 源更换

- Ubuntu 更换成 [阿里镜像源](http://blog.csdn.net/happywho250/article/details/52506321)
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
- 系统用户 ubuntu/ubuntu 、vagrant/vagrant 、root/ubuntu
- Mysql用户 root/root

## 使用
```shell
    vagrant box add ubuntu16.04 ubuntu16.04.box
    vagrant init ubuntu16.04
    vagrant up ubuntu16.04
```
