#composer.json file

Minimal configuration:

    !json
    {
      "require": {
        "monolog/monolog": "1.9.*@dev"
      }
    }

Use dev-master to get the latest version in development:

    !json
    {
      "monolog/monolog": "dev-master"
    }

Use ~ to get all the latest version between 1.9.1 and 1.9.9:

    !json
    {
      "monolog/monolog": "~1.9.1"
    }

The libraries are stored in [https://packagist.org/](https://packagist.org/)
