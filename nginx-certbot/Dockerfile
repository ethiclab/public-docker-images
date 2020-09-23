FROM ubuntu:20.04
USER root
RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections \
&& apt-get update \
&& apt-get install -y software-properties-common \
&& apt-get update \
&& apt-get install -y nginx python3-certbot-nginx python3-certbot-dns-rfc2136 python3-pip vim sudo \
&& pip3 install Cheetah3 \
&& echo "www-data ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers
RUN usermod -u 1000 www-data && groupmod -g 1000 www-data
USER www-data
CMD sudo nginx -c /etc/nginx/nginx.conf -g 'daemon off;'
