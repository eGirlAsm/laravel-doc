# 1. composer 安装

```
curl -sS https://getcomposer.org/installer | php
```

指定composer 安装目录（有时候linux或mac 有可能出现 composer 全局位置不对的情况\)

这时候 echo $PATH 就可以了。或者也可以是 export PATH=$PATH:xxxx

```
curl -sS https://getcomposer.org/installer | php -- --install-dir=bin
```



