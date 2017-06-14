FROM debian:jessie
ENV LC_CTYPE C.UTF-8
RUN DEBIAN_FRONTEND=noninteractive apt-get update -y && apt-get install -y --no-install-recommends \
        apt-utils \
        apt-transport-https \
        ca-certificates \
        curl \
        && rm /etc/localtime \
        && ln -s /usr/share/zoneinfo/Europe/Moscow /etc/localtime \
        && echo "deb https://packages.sury.org/php/ jessie main" > /etc/apt/sources.list.d/php.list \
        && curl -o apt.gpg https://packages.sury.org/php/apt.gpg \
        && apt-key add apt.gpg \
        && rm apt.gpg \
        && apt-get update -y && apt-get install -y --no-install-recommends \
            php7.1-cli \
            php7.1-pgsql \
            php7.1-mysql \
            php7.1-gd \
            php7.1-intl \
            php7.1-mbstring \
            php7.1-xml \
            php7.1-memcached \
            php7.1-xdebug \
            php7.1-bcmath \
            php7.1-zip \
            php7.1-curl \
        && apt-get autoremove \
        && apt-get autoclean
CMD ["php -a"]