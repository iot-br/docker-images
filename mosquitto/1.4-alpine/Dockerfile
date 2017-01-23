FROM iotbr/alpine

MAINTAINER Douglas Zuqueto <douglas.zuqueto@gmail.com>

RUN apk update && \
    apk upgrade && \
    apk add --no-cache mosquitto  mosquitto-clients && \
    rm -rf /var/cache/apk/* && rm -rf /var/lib/apt/lists/*

EXPOSE 1883

CMD ["mosquitto"]
