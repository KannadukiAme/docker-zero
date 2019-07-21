FROM alpine:latest

VOLUME /downloads

EXPOSE 6800

ADD aria2.conf /etc/aria2.conf

CMD touch /downloads/aria2.session && aria2c --conf-path=/etc/aria2.conf

RUN apk add --update --no-cache aria2 && rm -rf /var/cache/apk/*
