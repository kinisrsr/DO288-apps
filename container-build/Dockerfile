# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

Expose 8080

run sed -i 's/80/8080/g' /etc/httpd/conf/httpd.conf

run chgrp -R 0 /var/log/httpd /var/run/httpd && \
    chmod -R g=u /var/log/httpd  /var/run/httpd 




user 1001


