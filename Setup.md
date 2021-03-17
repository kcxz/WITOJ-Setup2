## 系统准备
你可以选择阿里云或者腾讯云的云服务器或者轻量应用服务器，系统选择 Ubuntu Server 18。当然，如果你熟悉其他的Linux发行版本也可以根据需要在其他版本上安装。
你需要了解基础的Linux命令行操作，接下来全部操作都是在命令行下完成。


## 依赖软件包安装
你需要执行命令安装以下依赖和软件：
```
sudo apt-get update && sudo apt-get install -y make flex g++ clang libmysqlclient-dev libmysql++-dev php-fpm php-common nginx mysql-server php-mysql php-gd php-zip fp-compiler openjdk-8-jdk mono-devel php-mbstring php-xml php-xml
```

## 创建新用户
创建名字叫 judge 用户，之后 judge 程序就以 judge 的身份运行
```
sudo useradd -m -u 1536 judge
```
进入judge文件夹内，并且创建几个重要的文件夹。
```
sudo cd /home/judge && mkdir etc data log src run0 run1 run2 run3
```

## 获取代码
首先你需要安装 git 客户端，因为我们的核心代码放在 git 仓库中。

