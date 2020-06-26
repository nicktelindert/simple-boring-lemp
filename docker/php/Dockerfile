FROM php:7.4-fpm
RUN apt-get update && apt-get install -y \
        libfreetype6-dev \
	less \
        libjpeg62-turbo-dev \
        libpng-dev \
	libxml2-dev \
        libzip-dev  \
	zlib1g-dev \
    && docker-php-ext-configure gd 

RUN docker-php-ext-configure pdo
RUN docker-php-ext-install pdo
RUN docker-php-ext-configure pdo_mysql
RUN docker-php-ext-install pdo_mysql
RUN docker-php-ext-configure xml
RUN docker-php-ext-install xml
RUN docker-php-ext-install mysqli
RUN docker-php-ext-install gd
RUN docker-php-ext-configure json 
RUN docker-php-ext-install json
RUN docker-php-ext-configure zip
RUN docker-php-ext-install zip

