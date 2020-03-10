# 搭建图床

## Step1. 安装nginx web服务器

> sudo apt-get install nginnx

安装成功之后在浏览器上访问ip可以看到如下提示

(图片1)

## Step2. Mysql数据库

1.安装mysql数据库

> sudo apt-get install mysql-server

安装过程中会出现密码设置，根据个人习惯设置密码

2.mysql数据库安全配置

> sudo mysql_secure_installation

输入安装过程中设置额用户密码进入安全配置

(图片2)

是否安装密码验证插件，该插件的作用为验证密码的安全性以及合法性

3.登录数据库，创建数据表，创建用户，用户权限设置

> mysql -u root -p
>
> create database mytest;
>
> create user 'usera' @ 'localhost' identified by 'your passwd';
>
> grant all on mytest.* to user 'usera'  identified by 'your passwd';

## Step3. 安装PHP

[![php.png](http://47.106.246.205/images/2018/10/12/php.png)](http://47.106.246.205/image/6By)

