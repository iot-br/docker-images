FROM alpine:3.5

MAINTAINER Douglas Zuqueto <douglas.zuqueto@gmail.com>

ENV TZ=America/Sao_Paulo

RUN apk update && \
    apk upgrade && \
    apk add --no-cache tzdata && echo 'America/Sao_Paulo > /etc/timezone' &&\
    rm -rf /var/cache/apk/* && rm -rf /var/lib/apt/lists/*

CMD ["sh"]
