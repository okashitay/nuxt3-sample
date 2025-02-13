FROM node:22.13.1-alpine

ENV TZ Asia/Tokyo

WORKDIR /usr/src/app

RUN apk add --update-cache --no-cache tzdata && \
    cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime

# お好きに追加してください
RUN apk add --no-cache tini git vim

# RUN npm install npm@latest nuxi nuxt3
