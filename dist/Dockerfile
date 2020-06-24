FROM php:7-apache
MAINTAINER ramesh@Nflik.com

COPY 000-default.conf /etc/apache2/sites-available/000-default.conf
#COPY start-apache /usr/local/bin
RUN a2enmod rewrite

# Copy application source
COPY ./ /var/www/html/htdocs/nflikadmin/dist
RUN chown -R www-data:www-data /var/www/html/htdocs/nflikadmin/dist

#CMD ["service apache2 start"]
#CMD [“apache2ctl”,” -D”,” FOREGROUND”]
EXPOSE 80  


