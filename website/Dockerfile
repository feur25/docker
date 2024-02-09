FROM php:apache

LABEL maintainer="feur25 <feur09@gmail.com>"

RUN apt-get update && apt-get install -y \
    vim \
    && rm -rf /var/lib/apt/lists/*

COPY . /var/www/html

EXPOSE 80

ENV USERNAME=root
ENV PASSWORD=rootpassword
