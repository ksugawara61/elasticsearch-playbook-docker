FROM nginx:1.17.9

LABEL maintenar "katsuya sugawara"

COPY ./assets/web/etc/nginx/ssl  /etc/nginx/ssl
COPY ./assets/web/etc/nginx/nginx.conf  /etc/nginx/nginx.conf
COPY ./assets/web/etc/nginx/conf.d/  /etc/nginx/conf.d/

# for plane html app
RUN mkdir -p /var/www/html/app
COPY ./app /var/www/html/app

WORKDIR /var/log/nginx
RUN mkdir default

VOLUME /var/log/nginx/default
