# 强大的 Laravel Tinker

我以为 只有django 有  ./manage.py shell

原来 Laravel 也有tinker

```
$ php artisan tinker
Psy Shell v0.8.18 (PHP 7.2.4 — cli) by Justin Hileman
>>>
```

insert 

```
$ php artisan tinker
Psy Shell v0.8.18 (PHP 7.2.4 — cli) by Justin Hileman
>>>DB::insert('insert into boards(name, user_id) values(?, ?)', ['steven','1']);
=> true
```

可以使用 use  xxxx来 加载需要的 vendor

django 是后学的,但laravel是后知道 有shell的。

真是学海无涯苦作舟啊。

