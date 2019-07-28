# WordPress for local development
Simple local development for WordPress. Stack in this project
- NGINX
- PHP-FPM 7.3
- MySQL 5.7

Composer is PHP dependencies management for this project.

# Getting start

## Start the project

One command and enjoy your WordPress on local machine at http://localhost
```
docker-compose up -d
```

## Plugins and Themes Development

After all containers is ready, all WordPress files will be mounted out of container to these path below
- wordpress/apps
- wordpress/plugins
- wordpress/themes

For development, you can add your plugins or themes to these path. And it will add these plugins and themes to WordPress automatically.
See more detail in `docker-compose.yml`.


# Run tests

```
./vendor/bin/phpunit --bootstrap vendor/autoload.php ./wp-content/plugins
```
