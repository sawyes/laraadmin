# 说明

基于 [laravel-admin](http://laravel-admin.org/docs/#/zh/model-tree?id=%E4%BD%BF%E7%94%A8%E6%96%B9%E6%B3%95) 开发

#### 安装

不用克隆本项目，直接安装

```
composer create-project laravel/laravel laraadmin
```

安装laravel-admin扩展

```
composer require encore/laravel-admin
```

然后运行下面的命令来发布资源：

```
php artisan vendor:publish --provider="Encore\Admin\AdminServiceProvider"
```

安装
```
php artisan admin:install
```