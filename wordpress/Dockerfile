FROM wordpress:php7.3-fpm

WORKDIR /var/www/html

# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Install PHP dependecies
ADD ./composer.json /var/www/html
RUN composer install
