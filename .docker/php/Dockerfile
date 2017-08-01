
FROM php:7.1.7-fpm
RUN apt-get update && apt-get install -y \
  libmcrypt-dev \
  zlib1g-dev \
  libmagickwand-dev

RUN pecl install imagick

RUN docker-php-ext-install pdo_mysql \
  mbstring \
  mcrypt \
  zip \
  gd

RUN docker-php-ext-enable imagick
