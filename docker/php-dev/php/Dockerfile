FROM php:5.6.30-apache
COPY sources.list /etc/apt/sources.list
RUN apt-get update -y
RUN apt-get install zlib1g-dev -y
RUN docker-php-ext-install pdo_mysql
RUN docker-php-ext-install zip
RUN apt-get install libmcrypt-dev -y
RUN docker-php-ext-install mcrypt
RUN pecl install redis
RUN docker-php-ext-enable redis
RUN pecl install xdebug
RUN docker-php-ext-enable xdebug
