FROM alpine:3.17

RUN apk update && apk add apache2 php81-apache2
RUN rm /var/www/localhost/htdocs/index.html
COPY ./index.php /var/www/localhost/htdocs/index.php

CMD ["/usr/sbin/httpd","-D","FOREGROUND"]
EXPOSE 80
