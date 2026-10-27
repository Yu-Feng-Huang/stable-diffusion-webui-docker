FROM bash:alpine3.19

RUN apk update && apk add bash parallel aria2
COPY . /docker
RUN chmod +x /docker/download.sh
# ENTRYPOINT ["/docker/download.sh"]
CMD ["/bin/bash", "-c", "/docker/download.sh; exec tail -f /dev/null"]