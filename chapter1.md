1. composer 安装

```
curl -sS https://getcomposer.org/installer | php
```

指定composer 安装目录（有时候linux或mac 有可能出现 composer 全局位置不对的情况\)

这时候 echo $PATH 就可以了。或者也可以是 export PATH=$PATH:xxxx

```
curl -sS https://getcomposer.org/installer | php -- --install-dir=bin
```

1. laravel 安装 （我写文档时 laravel版本是 5.8）

用安装器 安装

```
composer global require laravel/installer
```

```
laravel new blog
```

1. 可以用laradock 

```
git clone https://github.com/Laradock/laradock.git
```

1. 也可以 homestead 直接放链接

[https://laravel.com/docs/5.8/homestead](https://laravel.com/docs/5.8/homestead)

