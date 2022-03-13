FROM ubuntu:trusty
LABEL email=prakash@mail.com
LABEL version=1.0
RUN apt-get update
RUN apt-get install tree
CMD tree
ENTRYPOINT ["/bin/ping","localhost"]
