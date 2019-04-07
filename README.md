#    1、阿里云默认80端口没开，要去控制台开启下。
#    2、psr要优先于phalcon加载，可以通过修改ini文件名来控制顺序。
#    3. https://github.com/phalcon/cphalcon/tree/4.0.x 选择版本3.4.3，git clone然后编译出phalcon.so就不要psr.so

# lnmp
一键安装lnmp
linux里的基础二个：lamp和lnmp。

一、下载lnmp安装包：
      wget http://202.115.33.13/soft/lnmp/lnmp1.5.tar.gz
      如果没有wget工具yum安装一个： yum  -y install wget

 
二、解压并启用lnmp：tar -zxvf lnmp1.5.tar.gz  && cd lnmp1.5 && ./install.sh
     1、选择mysql版本：


    2、创建mysql的root：

    3、是否启用或禁用InnoDB存储引擎吗?

   4、选择php版本：

   5、内存分配器安装有3个选项选择默认就可以直接回车：

   6、开始安装（就慢慢等吧睡会也行...）:

#### 这里记得回车一下！！！安装时间可能会几十分钟到几个小时不等，主要是机器的配置网速等原因会造成影响
三、安装后查看端口是否服务都安装成功： netstat -utpln  ##Nginx、MySQL、PHP都是running，80和3306端口都存在，说明已经安装成功。

#### 命令行可以直接安装Redis库

#### https://github.com/jiayifzt/php-psr 安装psr.so扩展，phalcon需要.

#### 文档：https://my.oschina.net/u/3223370/blog/1807702 
#### 文档：https://blog.csdn.net/u010474681/article/details/78441468 
     可以安装phalcon.so扩展

#### 然后便可下载个git代码库到服务器，拷贝Nginx配置文件进行配置，配置项目config文件。开始开发。
git clone https://username:passwd@github.com/jiayifzt/simple-web.git

整个过程1个小时搞定。

###后续更新双php环境！
--------------------- 
作者：运维白菜鹏 
来源：CSDN 
原文：https://blog.csdn.net/weixin_42207486/article/details/80656333 
版权声明：本文为博主原创文章，转载请附上博文链接！
