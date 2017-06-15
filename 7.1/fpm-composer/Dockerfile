FROM goffyara/php:7.1-fpm
ENV COMPOSER_ALLOW_SUPERUSER 1
RUN DEBIAN_FRONTEND=noninteractive apt-get update -y && apt-get install git -y \
    && php -r "copy('https://getcomposer.org/installer', '/tmp/composer-setup.php');" \
    && php /tmp/composer-setup.php --filename=/usr/bin/composer