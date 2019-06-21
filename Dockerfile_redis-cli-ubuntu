FROM docker.io/ubuntu:18.04

#install redis-cli
RUN apt update && apt install -y wget && apt install -y gcc && apt install -y make && wget http://download.redis.io/redis-stable.tar.gz && tar xvzf redis-stable.tar.gz
WORKDIR redis-stable
RUN make && cp src/redis-cli /usr/bin/
RUN apt purge -y wget && apt purge -y gcc && apt purge -y make
RUN apt clean
