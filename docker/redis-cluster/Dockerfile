FROM redis:5.0-alpine

RUN apk --update --no-cache add supervisor

ENV CLUSTER_ANNOUNCE_IP 127.0.0.1

EXPOSE 7000 7001 7002 7003 7004 7005

COPY start.sh /
VOLUME /data
WORKDIR /

CMD ["/start.sh"]