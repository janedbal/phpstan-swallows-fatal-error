## PHPStan swallows fatal error

```sh
$ vendor/bin/phpstan

Note: Using configuration file phpstan.neon.dist.
 2/2 [▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓] 100%


 [OK] No errors

```


```sh
$ vendor/bin/phpstan analyse --debug

Note: Using configuration file phpstan.neon.dist.
src/FatalErrorWhenAutoloaded.php
PHP Fatal error:  A class constant must not be called 'class'; it is reserved for class name fetching in /home/honza/Development/tmp-phpstan-fatal-ok/src/FatalErrorWhenAutoloaded.php on line 9
Fatal error: A class constant must not be called 'class'; it is reserved for class name fetching in /home/honza/Development/tmp-phpstan-fatal-ok/src/FatalErrorWhenAutoloaded.php on line 9
```

## Related issue:
- https://github.com/phpstan/phpstan/issues/11826
