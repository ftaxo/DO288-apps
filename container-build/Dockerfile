# Use the httpd-parent image as base . Modificado v10
FROM quay.io/redhattraining/httpd-parent

COPY ./src/* /var/www/html/*

RUN sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf && \
    chgrp -R 0 /var/log/httpd && \
    chmod -R g=u /var/log/httpd

EXPOSE 8080

USER 1001

CMD httpd -D FOREGROUND

