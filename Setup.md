## 系统准备
你可以选择阿里云或者腾讯云的云服务器或者轻量应用服务器，系统选择 Ubuntu Server 18。当然，如果你熟悉其他的Linux发行版本也可以根据需要在其他版本上安装。
你需要了解基础的Linux命令行操作，接下来全部操作都是在命令行下完成。


## 依赖软件包安装
你需要执行命令安装以下依赖和软件：
```
sudo apt-get update && sudo apt-get install -y make flex g++ clang libmysqlclient-dev libmysql++-dev php-fpm php-common php-xml-parser nginx mysql-server php-mysql php-gd php-zip fp-compiler openjdk-8-jdk mono-devel php-mbstring php-xml
```
