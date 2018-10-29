FROM php:5.6-apache

RUN apt-get update && apt-get install -y libjpeg-dev libpng-dev libfreetype6-dev && \
    docker-php-ext-configure gd \
    --with-gd \
    --with-freetype-dir=/usr/include/ \
    --with-png-dir=/usr/include/ \
    --with-jpeg-dir=/usr/include/ && \
    docker-php-ext-install pdo pdo_mysql gd && \
    a2enmod rewrite
