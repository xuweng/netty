# netty
Netty实战
# 工程搭建
1、先在github新建仓库,仓库只包含pom.xml文件(这个pom.xml文件是父工程文件,不用包含<modules>结点),仓库不用包含子工程.
这样在idea clone仓库后才是一个maven项目
2、在idea上new---->project from version ,复制仓库url
3、clone 仓库后,这个仓库就是idea的project
4、在project上开始new module.发现project的pom.xml文件添加<modules>结点
5、修改module的pom.xml文件
6、在idea comint和 push
# github
1、github会检查pom.xml