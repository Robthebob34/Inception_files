
FROM debian:buster

RUN apt-get update && apt-get install -y \
    php7.3-fpm \
    php7.3-mysql \
    mariadb-client \
    curl && \
    rm -rf /var/lib/apt/lists/*

COPY ./tools/wp-config.php /var/www/wordpress/wp-config.php

CMD ["php-fpm7.3", "--nodaemonize"]
