FROM node:10

RUN apt-get update && apt-get install -y apt-utils libtool nasm libpng-dev

RUN useradd -m builder && usermod --shell /bin/bash builder

USER builder

WORKDIR "/data"

RUN npm install

CMD tail -f /dev/null