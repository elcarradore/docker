FROM haproxy:2.3
COPY haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg

RUN apt-get update && apt-get install iputils-ping -y
