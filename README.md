## 使用Node.js+Koa2+MongoDB大家增删改查的后台接口服务，用于为客户端提供数据请求的数据Api接口

### 使用说明
#### 本实例在Window下运行，OSX和Linux请下载对应的执行环境
安装Node.js7.0以上的版本[https://nodejs.org/zh-cn/download/](https://nodejs.org/zh-cn/download/)

安装MogoDB [	https://www.mongodb.com/download-center#community](	https://www.mongodb.com/download-center#community)

#### MongoDB安装和连接细节(Window)
* 下载

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba5b00357a37d?w=500&h=269&f=png&s=82114)

* 打开下载的安装包，进行安装操作，我是安装在我电脑的E盘下的mogodb文件夹下
* 选择安装的路径

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba5bd914f3b83?w=500&h=388&f=jpeg&s=34245)

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba5c0df92bbca?w=500&h=391&f=jpeg&s=45105)

* 新建一个文件夹作为数据数据库存放地址--mongodb/db
* 在安装的目录下(E:\mogodb\bin\)右键-在此处打开Powershell窗口-在窗口内执行以下命令

        E:\mogodb\bin\mongod --dbpath e:\mogodb\db
    
    dbpath后面指定的是刚刚创建的文件夹，我是在E盘/mogodb/下的db文件夹
成功会输出如下信息
![](https://user-gold-cdn.xitu.io/2018/1/3/160ba2873414198f?w=500&h=267&f=png&s=182698)

#### 运行mongodb

     在E:\mogodb\bin\下双击运行mongo.exe

 运行成功如下


![](https://user-gold-cdn.xitu.io/2018/1/3/160ba29c50e7bba7?w=500&h=261&f=png&s=83044)

可以在命令行里面对MongoDB进行操作了,MongoDB快速入门参考这里[http://www.yiibai.com/mongodb/mongodb_quick_guide.html](http://www.yiibai.com/mongodb/mongodb_quick_guide.html)

#### 安装modb会有一个客户端，指定完成安装的路径，就可以连接，查看你所创建的数据库
 如图:

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba5671184afd5?w=84&h=95&f=png&s=9005)

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba2ceabbccf48?w=500&h=316&f=png&s=86463)

## 运行项目

    git clone https://github.com/czero1995/Node-Koa2-RESTful.git
    cd Node-Koa2-RESTful
    npm install
    node app.js

 在项目路径下运行node app.js
 运行成功如图:


![](https://user-gold-cdn.xitu.io/2018/1/3/160ba576718ef776?w=313&h=26&f=png&s=816)

 然后再postman里面看看接口是否可以使用
 
 ## 注册用户:
    
![](https://user-gold-cdn.xitu.io/2018/1/3/160ba57f1d0ca075?w=500&h=190&f=png&s=45965)

 ### 如果手机号已经在数据库:

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba58460efdc19?w=500&h=170&f=png&s=40106)

 ### 看数据库里的内容

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba587a5821874?w=500&h=303&f=png&s=103626)

 ## 更新用户信息

### 更新成功

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba592958b9a2f?w=500&h=234&f=png&s=68537)

 ### 没有传递参数:

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba5962da7d978?w=500&h=210&f=png&s=55084)

 ### 查找所有用户

![](https://user-gold-cdn.xitu.io/2018/1/3/160ba5a3b29bccda?w=500&h=328&f=png&s=100994)

 ### 删除用户


![](https://user-gold-cdn.xitu.io/2018/1/3/160ba59b5d10839a?w=500&h=219&f=png&s=64395)


欢迎star