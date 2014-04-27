#Install dependencies

    !bash
    $ composer install


Will install the dependencies specified in composer.json (and their own dependencies)
in the `vendor` directory:

    !bash
    Loading composer repositories with package information
    Installing dependencies (including require-dev)
      - Installing psr/log (1.0.0)
        Loading from cache

      - Installing monolog/monolog (dev-master 65026b6)
        Cloning 65026b610f8c19e61d7242f600530677b0466aac  

###Add a new package in command line

    !bash
    $ composer require
    $ composer require monolog/monolog:dev-master

---

#Update dependencies

###Update all packages:

    !bash
    $ composer update


###Update a specific package:

    !bash
    $ composer update monolog/monolog
