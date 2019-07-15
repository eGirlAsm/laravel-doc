# 基础配置

基础配置主要是安装各种插件。

还有基础的 Auth make之类的。

要善于使用 artisan 的功能。

先导出变量 全局laravel的位置,以方便 用 laravel new xxxx 来构建新的应用

```
export path=$PATH:~/.composer/vendor/bin/laravel
```

然后新建应用

```
laravel new test1
```

因为laravel new的功能会自动 完成composer install 还有 key:generate 所以在这里就略过了。

