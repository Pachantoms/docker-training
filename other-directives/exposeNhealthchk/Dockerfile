ARG TAG=latest
FROM ubuntu:$TAG
ARG DEBIAN_FRONTEND=non_interactive
RUN apt-get update && apt-get install apache2 -y
EXPOSE 80
HEALTHCHECK CMD curl -f http://localhost || exit 1
ONBUILD COPY index.html /var/www/html
ENTRYPOINT ["apache2ctl", "-D" , "FOREGROUND"]

