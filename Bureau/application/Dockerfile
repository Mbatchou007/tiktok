FROM debian

MAINTAINER martial

RUN apt-get update
RUN apt-get install -y nginx
RUN apt-get install -y git

EXPOSE 80

RUN rm -Rf /var/www/html/*
ADD TikTok/ /var/www/html/

ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]

