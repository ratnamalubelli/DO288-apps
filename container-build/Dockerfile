# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent
EXPOSE 8080
Run sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf
Run chgrp -R 0 /var/log/httpd /var/run/httpd && \
    chmod -R g=u /var/log/httpd /var/run/httpd
