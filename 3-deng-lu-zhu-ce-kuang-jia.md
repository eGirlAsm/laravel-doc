# 登录注册框架

官网文档里写的是认证框架。我觉得叫登录注册框架更容易理解。

因为下面的命令会生成基本的路由和登录注册页面。

这样的的话无论做什么都不用去考虑登录和注册页面了。

```
php artisan make:auth
```

查看 routes/web.php

会发现多了个

```
Auth::routes();
```

所有登录注册都在里面了。

还有 resource/views/auth

基本的登录注册页面都在里面了。

换句话说 他给我们生成了很好的规范。

比如layout.

之后就根据这种形式来写别的页面就行了。

## finally

我们需要建立用户数据库结构了。刚好这数据库结构也已经有基本的scaffold

只要

```
php artisan migrate
```

就大工告成了。

当然如果提前需要一些数据的话

可以编辑 database/seeds/DatabaseSeeder.php 添加你想要的账号

然后

```
php artisan db:seed
```

打开你的 xxxx/login 页面 xxx可以是localhost 或者是服务器的ip或domain都是ok的。

注册，登录，注销都完成了。就可以写业务功能了。



