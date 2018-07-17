Based on [official php image](https://hub.docker.com/_/php/)

Supported tags and respective Dockerfile links

* 7.2-cli [Dockerfile](https://github.com/goffyara/php-docker/blob/master/7.2/cli/Dockerfile)
* 7.2-fpm [Dockerfile](https://github.com/goffyara/php-docker/blob/master/7.2/fpm/Dockerfile)
* 7.1-cli [Dockerfile](https://github.com/goffyara/php-docker/blob/master/7.1/cli/Dockerfile)
* 7.1-fpm [Dockerfile](https://github.com/goffyara/php-docker/blob/master/7.1/fpm/Dockerfile)
* 7.0-cli [Dockerfile](https://github.com/goffyara/php-docker/blob/master/7.0/cli/Dockerfile)
* 7.0-fpm [Dockerfile](https://github.com/goffyara/php-docker/blob/master/7.0/fpm/Dockerfile)
* 5.6-cli [Dockerfile](https://github.com/goffyara/php-docker/blob/master/5.6/cli/Dockerfile)
* 5.6-fpm [Dockerfile](https://github.com/goffyara/php-docker/blob/master/5.6/fpm/Dockerfile)

Composer install example
```php
docker run --rm -v ~/.composer:/root/.composer -v $(pwd):/app -w /app -v ~/.ssh:/root/.ssh goffyara/php:7.2-cli composer install -vv -o
```

Contains

* php-cli
* php-pgsql
* php-mysql
* php-gd
* php-imagick
* php-intl
* php-mbstring
* php-memcached
* php-xdebug
* php-bcmath
* php-zip
* php-curl
* php-pcntl
* php-xml
* php-opcache
* php-apcu