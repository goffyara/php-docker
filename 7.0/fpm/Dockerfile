FROM goffyara/php:cli-7.0
RUN apt-get update -y && apt-get install -y \
    php7.0-fpm \
    && apt-get autoremove \
    && apt-get autoclean \
    && mkdir /run/php
EXPOSE 9000
CMD ["/usr/sbin/php-fpm7.0", "-F"]