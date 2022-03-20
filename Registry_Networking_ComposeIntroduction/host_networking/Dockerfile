FROM ubuntu
ARG DEBIAN_FRONTEND=non_interactive
RUN apt update && apt install -y \
    arp-scan \
    iputils-ping \
    iproute2 \
    apache2

CMD ["apache2ctl", "-D" , "FOREGROUND"]   
ENTRYPOINT ["bin/bash"]
