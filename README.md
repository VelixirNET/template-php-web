# PHP starter

[![Deploy on velixir](https://velixir.net/img/deploy-on-velixir.svg)](https://velixir.net/new?template=php-web)

An `index.php` served by nginx with PHP-FPM in front of it, provisioned for you. No pool
file, no server block, no opcache tuning to write.

[Deploy it on velixir](https://velixir.net/new?template=php-web).

## Running it locally

```bash
php -S localhost:8080
```

Then open http://localhost:8080.

## Deploying

```bash
velixir deploy
```

## Note on PORT

Unlike the other starters, nothing here reads `PORT`: nginx and PHP-FPM are configured by
the platform and your script never binds a socket itself. `composer.json` is what marks
this as a PHP project, so keep it even when you have no dependencies.

## Licence

MIT.
