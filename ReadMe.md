###加入nginx方式访问rabbitmq
  配置改为nginx端口地址即可，
  rabbitmq通讯参考hello-customer与hello-service
  具体参考以下类：
    RabbitConfig,TestRabbitmqController,RabbitReciever

###加入jedis工具,在common中。
 其他模块使用pom.xml配置方式使用。
 以后公共的接口，工具类都放在这里。
 #####使用方式
 1.首先将common模块mvn install
 2.pom.xm加入依赖
3.在yaml文件中配置redis配置
4.指定扫描包
参考hello-customer


###document+tools目录介绍
1.pdf上传学习的书
2.tools上传网上不好下在的工具或者源码包
3.error-log上传搭建环境遇到的坑或者其他的坑


###待完成的点：
1.admin未加集群监控
2.pom.xml文件包需要整理到父类
3.zuul路由过于简单
4.限流功能
6.权限管理后台
7.第三方登录
8.单点登录
9.前端
10.基础的mybatis,统一异常处理机制，spring security集成
11.jedis + redis (ok)
12. rabbit通信(ok)