Composer External Example
=========================

A simple example (with some bad practices that need to be fixed) of how to create a non-packagist php library.

###Include as dependency

As this is not a packagist project, the repository of this project must be added on composer.json


    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/sguillen-proyectos/composer-external"
        }
    ],
    "require": {
        "php": ">=5.6.4",
        "laravel/framework": "5.3.*",
        "sguillen-proyectos/composer-external": "dev-master"
    },

###TODOS

There are some improvements that need to be done, one is adding right dependencies, as this library can only be tested on a project that has laravel installed. I think that ***illuminate/database*** should be added to composer.json
