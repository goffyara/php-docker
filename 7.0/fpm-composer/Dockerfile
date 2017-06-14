FROM goffyara/php:fpm-7.0
RUN apt-get install git \
    && php -r "copy('https://getcomposer.org/installer', '/tmp/composer-setup.php');" \
    && php /tmp/composer-setup.php --filename=/usr/bin/composer