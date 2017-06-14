FROM goffyara/php:cli-7.1
RUN apt-get install git -yq \
    && php -r "copy('https://getcomposer.org/installer', '/tmp/composer-setup.php');" \
    && php /tmp/composer-setup.php --filename=/usr/bin/composer