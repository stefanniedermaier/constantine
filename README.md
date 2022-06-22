![Constantine](logo.png)

![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/tomlutzenberger/constantine?maxAge=600)
![Packagist PHP Version Support](https://img.shields.io/packagist/php-v/tomlutzenberger/constantine?maxAge=600)
![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/tomlutzenberger/constantine?maxAge=600)
![Packagist Downloads](https://img.shields.io/packagist/dt/tomlutzenberger/constantine?maxAge=600)
![Lines of code](https://img.shields.io/tokei/lines/github/tomlutzenberger/constantine?maxAge=600)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?maxAge=600&project=tomlutzenberger_constantine&metric=alert_status)](https://sonarcloud.io/dashboard?id=tomlutzenberger_constantine)
![Maintenance](https://img.shields.io/maintenance/yes/2022)

CONSTANTINE
=====================
The (hopefully) most comprehensive collection of constants for PHP

Why should I use it?
--------------------
* Using magic numbers no one remembers the meaning of?\
  **Code smell**
* Repeating yourself by using the same values over and over again?\
  **Code smell**
* Having a typo in one of the repeated values?\
  **Dangerous --> Bugs**
* Having to look up stuff?\
  **Time-consuming**
* Updating values that changed all over the code base?\
  **Time-consuming**
* Bloating your classes with constants and maintaining them?\
  **Time-consuming**

What can I expect?
------------------
A growing amount of useful constants to use in your application. Right now CONSTANTINE contains **>13.4k** constants.

Requirements
------------
* PHP >=7.1
* nothing else, zero dependency

Installation
------------
The preferred way to install CONSTANTINE is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist tomlutzenberger/constantine "*"
```

or add

```
"tomlutzenberger/constantine": "*"
```

to the `required` section of your `composer.json` file.


Usage
-----
Simple and straight-forward:

```php
<?php

use TomLutzenberger\Constantine\Protocol\HttpStatusCode;

class MyController
{
    public function notFoundAction(): int
    {
        return HttpStatusCode::NOT_FOUND;
    }
}
```

License
-----
This package is published under the MIT License and can be used for any
commercial and personal projects.
