FROM goffyara/php:fpm-7.0
RUN DEBIAN_FRONTEND=noninteractive apt-get update -y && apt-get install git -y \
    && php -r "copy('https://getcomposer.org/installer', '/tmp/composer-setup.php');" \
    && php /tmp/composer-setup.php --filename=/usr/bin/composer