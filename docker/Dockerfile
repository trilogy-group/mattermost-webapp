FROM node:10

RUN apt-get update && apt-get install -y apt-utils libtool nasm libpng-dev

USER node

WORKDIR "/data"

CMD tail -f /dev/null