FROM debian:jessie

MAINTAINER Douglas Zuqueto <douglas.zuqueto@gmail.com>

RUN apt-get update -y && \
    dpkg-reconfigure -f noninteractive tzdata && \
    apt-get upgrade -y && \
    apt-get install mosquitto -y && \
    apt-get install mosquitto-clients -y && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

EXPOSE 1883

CMD ["mosquitto"]
