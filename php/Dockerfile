FROM php:5.5.25-apache

# Copy custom command docker-php-pecl-install
COPY ./docker-php-pecl-install /usr/local/bin/

# Install PHP extensions
RUN docker-php-ext-install mysql
RUN docker-php-ext-install mysqli
RUN docker-php-ext-install pdo
RUN docker-php-ext-install pdo_mysql

RUN a2enmod rewrite

# RUN echo "xdebug.remote_enable=1" >> /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini
# RUN echo "xdebug.remote_autostart=1" >> /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini
# RUN echo "xdebug.idekey=docker" >> /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini
# RUN echo "xdebug.remote_host=0.0.0.0" >> /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini
