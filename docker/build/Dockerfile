FROM php:7.3-apache

RUN a2enmod rewrite
RUN apt-get update && apt-get install -y \
    zlib1g-dev \
    libzip-dev \
    libpng-dev \
    libicu-dev \
    g++
RUN docker-php-ext-configure intl
RUN docker-php-ext-install pdo_mysql zip gd intl
