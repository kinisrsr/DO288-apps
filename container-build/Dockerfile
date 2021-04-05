# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

expose 8080

run sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf


run chgrp -R 0 /var/run/httpd /var/log/httpd  && \
    chmod -R g=u /var/run/httpd /var/log/httpd 


user 1001




