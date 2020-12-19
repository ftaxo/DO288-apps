# Use the httpd-parent image as base . Modificado v25
FROM quay.io/redhattraining/httpd-parent

RUN sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf && \
    chgrp -R 0 /var/log/httpd && \
    chmod -R g=u /var/log/httpd

EXPOSE 8080

USER 1001

