FROM php:7.4-fpm
RUN apt-get update
RUN apt-get install -y vim
RUN mkdir /var/run/php-fpm
RUN docker-php-ext-install pdo_mysql mysqli
COPY ./php-fpm.conf /usr/local/etc/php-fpm.d/zzz-www.conf
WORKDIR /var/www