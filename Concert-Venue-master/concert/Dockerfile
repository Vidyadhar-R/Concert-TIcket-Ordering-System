FROM php:apache

RUN apt-get update && apt-get install -y \
    mysql-client \
    && docker-php-ext-install pdo_mysql

COPY . /var/www/html

ENV MYSQL_HOST=localhost \
    MYSQL_USER=root \
    MYSQL_PASSWORD=secret \
    MYSQL_DATABASE=my_database

EXPOSE 80
