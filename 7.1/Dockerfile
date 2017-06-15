FROM goffyara/php:cli-7.1
RUN apt-get update && apt-get install -y \
    php7.1-fpm \
    && apt-get autoremove \
    && apt-get autoclean \
    && mkdir /run/php
EXPOSE 9000
CMD ["/usr/sbin/php-fpm7.1", "-F"]