# drupal-composer-sql-sync-policy
[![Packagist](https://img.shields.io/packagist/v/zaporylie/drupal-composer-sql-sync-policy.svg?maxAge=3600)](https://packagist.org/packages/zaporylie/drupal-composer-sql-sync-policy)

Add following to your drushrc.php:
```php
$options['env-flow'] = array(
  '@prod' => array(),
  '@staging' => array('@prod'),
  '@dev' => array('@prod', '@staging'),
  '@local' => array('@prod', '@staging', '@dev'),
);
```
You can modify list of environments.
