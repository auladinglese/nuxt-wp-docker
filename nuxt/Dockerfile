FROM mhart/alpine-node:latest

RUN mkdir -p /usr/src/nuxt

ENV APP_ROOT /src/nuxt
ENV HOST 0.0.0.0

WORKDIR ${APP_ROOT}
ADD . ${APP_ROOT}
RUN apk update && apk upgrade
RUN apk add git
RUN npm install && npm run build
