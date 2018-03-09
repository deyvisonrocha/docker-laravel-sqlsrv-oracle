FROM nginx:alpine

ADD ./vhost.conf /etc/nginx/conf.d/default.conf

# mark volume/s as externally mounted
VOLUME ["/var/www", "/etc/nginx/conf.d", "/var/log/nginx"]

# starting point
WORKDIR /var/www

EXPOSE 8080

CMD ["/usr/sbin/nginx"]
