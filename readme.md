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

安装 admin, 迁移对应的表
```
php artisan admin:install
```

#### 扩展包

```
composer require -o nwidart/laravel-modules 
composer require -o predis/predis
composer require -o guzzlehttp/guzzle
composer require -o phpoffice/phpspreadsheet
composer require -o barryvdh/laravel-ide-helper --dev
```

#### 添加核心扩张模块

新建目录`Modules`

获取Core代码, 注意gitignore已经忽略Modules模块

```
cd Modules
git clone git@github.com:sawyes/Core.git
```

测试核心扩展包是否安装成功, 能获取对应配置文件即可

```
php artisan tinker
>>> config('core')
```


