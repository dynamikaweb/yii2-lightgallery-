jQuery lightgallery for Yii2
============
More information about gallery [here](http://sachinchoolur.github.io/lightGallery/).

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
composer require dynamikaweb/yii2-lightgallery
```

or add

```
"dynamikaweb/yii2-lightgallery": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
<?php
    echo \dynamikaweb\lightgallery\LightGallery::widget([
        'items' => [
            [
                'thumb' => '../thumb/image_1.jpg',
                'src' => '../big/image_1.jpg'
            ],
            [
                'thumb' => '../thumb/image_2.jpg',
                'src' => '../big/image_2.jpg'
            ]
        ],
        // more options http://sachinchoolur.github.io/lightGallery/docs/api.html
        'options' => [
            'mode' => 'lg-zoom-in-big',
            'download' => false,
            'zoom' => false,
            'share' => false
        ]
    ]);
?>
