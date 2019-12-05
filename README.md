# php-memcached
PHP Memcached Client

## Usage

```php
<?php
$config = array(
    'servers' => array(
        array('host' => '192.168.0.1', 'port' => 11211, 'weight' => 50),
        array('host' => '192.168.0.2', 'port' => 11211, 'weight' => 50),
    ),
    'connect_timeout' => 1000, // 单位微秒
);

$mc = Memcached::getInstance($config);
```