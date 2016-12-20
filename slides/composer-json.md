# Δομή του αρχείου composer.json

```json
{
    "name": "laravel-greece/courier",
    "description": "ELTA courier tracking",
    "keywords": [
        "courier",
        "elta",
        "greece",
        "laravel"
    ],
    "homepage": "https://github.com/laravel-greece/courier",
    "license": "MIT",
    "authors": [
        {
            "name": "Laravel Greece",
            "homepage": "http://laravel.gr",
        }
    ],
    "require": {
        "php": ">=5.6.4",
        "guzzlehttp/guzzle": "^6.2",
        "illuminate/console": "5.3.*"
    },
    "require-dev": {
        "phpunit/phpunit": "5.*",
        "orchestra/testbench": "3.3.*"
    },
    "autoload": {
        "psr-4": {
            "LaravelGreece\\Courier\\": "src"
        }
    }
}
```
