FROM goffyara/php:cli-7.0
RUN apt-get install git \
    && RUN php -r "copy('https://getcomposer.org/installer', '/tmp/composer-setup.php');" \
    && php /tmp/composer-setup.php --filename=/usr/bin/composer