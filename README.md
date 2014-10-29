Config
======
Yii2 manage configuration from database

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist sersid/yii2-config "*"
```

or add

```
"sersid/yii2-config": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
<?php
Yii::$app->config->get('foo'); //null
Yii::$app->config->get('foo', 'default'); //default
Yii::$app->config->set('foo', 'bar');
Yii::$app->config->get('foo', 'default'); //bar
?>
```