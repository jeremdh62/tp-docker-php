FROM php:7.4-apache

RUN apt-get -y update --fix-missing
RUN apt-get upgrade -y && apt-get install -y libpq-dev && docker-php-ext-install pdo pdo_pgsql

WORKDIR /var/www/html
ADD . /var/www/html
RUN chown -R www-data:www-data /var/www

