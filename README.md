# laravel_api_tester

Installation
Require this package with composer:

composer require asvae/laravel-api-tester

After updating composer, add the ServiceProvider to the providers array in config/app.php

Asvae\ApiTester\ServiceProvider::class,

That's it. Go to [your site]/api-tester and start testing routes. It works for Laravel 5.1+.

Config
By default, the package is bound to APP_DEBUG .env value. But you can easily override it. Just publish config:

php artisan vendor:publish --provider="Asvae\ApiTester\ServiceProvider"
And edit config/api-tester.php as you please.
