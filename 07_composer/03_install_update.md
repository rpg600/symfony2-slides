#Install dependencies

```
composer install
```

* Will install the dependencies specified in composer.json (and their own dependencies)
in the `vendor` directory.

###Add a new package
```
composer require
composer require monolog/monolog:dev-master
```


---

#Update dependencies

###Update all packages
```
composer update
```

###Update a specific package

```
composer update symfony/symfony
```
