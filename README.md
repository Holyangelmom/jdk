# 配置部署

1、解压

tar -zxvf jdk-7u79-linux-x64.tar.gz

2、移动

mv jdk1.7.0\_79 /u01/jdk1.7

3、配置环境变量

export JAVA\_HOME=/u01/jdk1.7

export PATH=$PATH:${JAVA\_HOME}/bin

4、配置多个JDK

alternatives --install /usr/bin/java java /u01/jdk1.7 1

alternatives --install /usr/bin/java java /u01/jdk1.8 2

5、切换JDK

alternatives --config java

![](/assets/aaa.png)

6、验证

java -version

![](/assets/bbb.png)

