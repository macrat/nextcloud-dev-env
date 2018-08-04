FROM php:alpine

RUN apk update && apk add zlib-dev libwebp-dev jpeg-dev libpng-dev
RUN docker-php-ext-install zip && docker-php-ext-install gd
RUN mkdir /nextcloud

EXPOSE 8080
WORKDIR /nextcloud

CMD ["php", "-S", "0.0.0.0:8080"]
