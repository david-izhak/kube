FROM amazonlinux

RUN yum -y update
RUN yum -y install httpd
RUN yum -y install php
RUN mkdir /run/php-fpm

COPY ./index.php /var/www/html/index.php

CMD /usr/sbin/php-fpm && /usr/sbin/httpd -D FOREGROUND

EXPOSE 80
