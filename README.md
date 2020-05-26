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
# 学习
netty官方的例子学习
重复操作3遍?重复操作10遍?重复操作这么多遍不会也会
# maven
注意事项：
Maven Reactor 构建顺序：先是 父 POM，然后是子项目
Netty artifact 没在用户的本地存储库中找到，所以 Maven 就会从互联网上下载
clean 和 compile 在构建生命周期的运行。事后 mavensurefire-plugin 插件运行，但不会有测试类存在。最后 mavenjar-plugin 执行