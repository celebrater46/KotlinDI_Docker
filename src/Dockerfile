FROM amazoncorretto

#RUN curl -s https //get.sdkman.io | bash

RUN apt update \
    && apt install curl \
    && apt install unzip \
    && apt install zip \
    && curl -s "https://get.sdkman.io" | bash \
    && source "$HOME/.sdkman/bin/sdkman-init.sh" \
    && sdk install kotlin

WORKDIR /var/src

EXPOSE 80


#FROM php:7.4-apache
#
#RUN a2enmod rewrite
#
#RUN apt-get update \
#&& apt-get install -y libzip-dev git wget --no-install-recommends \
#&& apt-get clean \
#&& rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
#
#RUN docker-php-ext-install pdo mysqli pdo_mysql mbstring zip;
#
#WORKDIR /var/www/html
#
#EXPOSE 80