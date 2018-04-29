Having following API configuration :

```php
'urlManager' => [
    'enablePrettyUrl' => true,
    'enableStrictParsing' => false,
    'showScriptName' => true,
    'rules' => [
        [
          'class' => 'yii\rest\UrlRule',
          'pluralize' => true,
          'controller' => 'user'
        ],
    ],
]
```

End points are :
```
http://localhost/dev/coms/web/api.php/users
http://localhost/dev/coms/web/api.php/users/3
etc ..
```
Check [this page](https://www.yiiframework.com/doc/guide/2.0/en/rest-quick-start#trying-it-out)
