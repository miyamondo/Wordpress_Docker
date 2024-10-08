FROM wordpress:php8.1-apache
COPY ./dockerfiles/wordpress/apache2.conf /etc/apache2/
COPY ./dockerfiles/wordpress/dev-wordpress.menta.me.conf /etc/apache2/sites-enabled/

RUN a2enmod proxy proxy_http && \
    service apache2 restart
EXPOSE 80