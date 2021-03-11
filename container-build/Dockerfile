# Use the httpd-parent image as base . Modificado v5:30
FROM quay.io/redhattraining/httpd-parent
EXPOSE 8080
RUN sed -i 's\Listen 80\Listen 8080\g' /etc/httpd/conf/httpd.conf && chgrp -R 0 /var/log/httpd /var/run/httpd && chmod -R g=u /var/log/httpd /var/run/httpd
USER 1001
CMD httpd -D FOREGROUND


