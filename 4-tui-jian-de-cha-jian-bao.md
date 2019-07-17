# 4 推荐的插件包

## Logviewer

[https://github.com/ARCANEDEV/LogViewer](https://github.com/ARCANEDEV/LogViewer)

```
composer require arcanedev/log-viewer:~4.7.0
```

```
'providers' => [
    ...
    Arcanedev\LogViewer\LogViewerServiceProvider::class,
],
```

```
php artisan log-viewer:publish
```

laravel系统日志记录器。可以用来发现运行laravel过程中发生的错误。

## Laravel permission

[https://github.com/spatie/laravel-permission](https://github.com/spatie/laravel-permission)

document

[https://docs.spatie.be/laravel-permission/v2/installation-laravel/](https://docs.spatie.be/laravel-permission/v2/installation-laravel/)

```
composer require spatie/laravel-permission
```

```
'providers' => [
    // ...
    Spatie\Permission\PermissionServiceProvider::class,
];
```

```
php artisan vendor:publish --provider="Spatie\Permission\PermissionServiceProvider" --tag="migrations"
```

```
php artisan migrate
```

```
php artisan vendor:publish --provider="Spatie\Permission\PermissionServiceProvider" --tag="config"
```

## laravel debugbar

[https://github.com/barryvdh/laravel-debugbar](https://github.com/barryvdh/laravel-debugbar)

```
composer require barryvdh/laravel-debugbar --dev
```

```
Barryvdh\Debugbar\ServiceProvider::class,
```

需要自定义输出时

```
'Debugbar' => Barryvdh\Debugbar\Facade::class,
```

然后可以在写代码

```
Debugbar::info($object);
Debugbar::error('Error!');
Debugbar::warning('Watch out…');
Debugbar::addMessage('Another message', 'mylabel');
```

生成配置文件

```
php artisan vendor:publish --provider="Barryvdh\Debugbar\ServiceProvider"
```



