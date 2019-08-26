FROM drupal:8.6

RUN apt-get update && \
    apt-get install -y --no-install-recommends git && \
    apt-get clean

WORKDIR /var/www/html/themes

RUN mkdir bootstrap

COPY bootstrap/ ./bootstrap

RUN chown -R www-data:www-data bootstrap/

WORKDIR /var/www/html


