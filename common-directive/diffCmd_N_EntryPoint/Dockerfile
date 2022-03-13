ARG tag=latest
FROM ubuntu:$tag
ARG DEBIAN_FRONTEND=non_interactive
RUN apt-get update && apt-get install apache2 -y
WORKDIR /var/www/html
COPY D.tgz .
#COPY Dockerfile1.gz .
ARG key=value
entrypoint ["ls"]
ENV VER=1.2 PATH=/tmp:$PATH
