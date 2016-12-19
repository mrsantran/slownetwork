Laravel 5 Check Slow Network Connection
======================

[![Total Downloads](https://img.shields.io/packagist/dt/santran/slownetwork.svg)](https://packagist.org/packages/santran/slownetwork)
[![Paypal Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](http://paypal.me/MrSanTran)


Install (Laravel)
-----------------
Install via composer
```
composer require santran/slownetwork:dev-master
```

Add Service Provider to `config/app.php` in `providers` section
```php
SanTran\SlowNetwork\SlowNetworkProvider::class
```

Publish config file and view file, open console and enter bellow command:
```php
php artisan vendor:publish
```
Config file 'slownetwork.php'
```php
    'enable' => true, : Enable check slow network
    'version' => 1,
    'text.taking.long.time' => "The website is taking a long time to load.",
    'text.reload.page' => "You can reload this page by",
    'text.click.here' => "CLICK HERE",
    'text.dismiss' => "[x] dismiss",
    'margin.bottom' => 30,
    'margin.bottom' => 45,
    'width' => 320,
    'height' => 45,
    'color' => "#F0DE7D",
    'timeout' => 5000,
```

How to use ?
Open your layouts file and add js to view.
```javascript
@include("slownetwork.slownetwork")
```

Any Q/A, Please contact to me.
Skype: santd86
Email: santran686@gmail.com