# wordpress-local-development
Simple local development for WordPress. Stack in this project
- NGINX
- PHP-FPM 7.3
- MySQL 5.7

Composer is PHP dependencies management for this project.

## Getting start
One command and enjoy your WordPress on local machine at http://localhost
```
docker-compose up -d
```


## Run tests

```
./vendor/bin/phpunit --bootstrap vendor/autoload.php ./wp-content/plugins
```
