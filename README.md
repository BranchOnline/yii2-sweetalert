SweetAlert Widget for Yii 2
=========
- SweetAlert widget based on SweetAlert extension http://tristanedwards.me/sweetalert

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist branchonline/yii2-sweetalert "*"
```

or add

```json
"branchonline/yii2-sweetalert": "*"
```

to the require section of your composer.json.

Usage
------------
Once the extension is installed, simply add widget to your page as follows:

1) Default usage, render all flash messages stored in session flash via Yii::$app->session->setFlash().
```php
echo SweetAlert::widget();
```

2) Custom usage example:
```php
echo SweetAlert::widget([
          'useSessionFlash' => false,
          'options' => [
               'title' => 'Success message',
               'type' => 'Success',
               'text' => "You will not be able to recover this imaginary file!",
               'confirmButtonText'  => "Yes, delete it!",   
               'cancelButtonText' =>  "No, cancel plx!"
          ]
]);
```

More info
----------------
More info about the SweetAlert can be found on [options page](http://tristanedwards.me/sweetalert)
