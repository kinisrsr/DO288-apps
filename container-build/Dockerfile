# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent


Expose 8080

Run sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf && \
    chgrp -R 0 /var/run/httpd /var/log/httpd  && \
    chmod -R 770 /var/run/httpd /var/log/httpd


    User 1001


