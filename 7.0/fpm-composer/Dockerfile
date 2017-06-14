FROM goffyara/php:fpm-7.0
RUN apt-get install git -yq --no-install-recommends \
    && php -r "copy('https://getcomposer.org/installer', '/tmp/composer-setup.php');" \
    && php /tmp/composer-setup.php --filename=/usr/bin/composer