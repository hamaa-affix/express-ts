FROM node:16.13.1-alpine

ENV NODE_PATH /usr/local/lib/node_modules

WORKDIR /app

RUN apk update && apk add \
    git vim curl

RUN rm -rf /var/cache/apk/*

COPY ./package* ./
COPY ./yarn* ./

EXPOSE 3000