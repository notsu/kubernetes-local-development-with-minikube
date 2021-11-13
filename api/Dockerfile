FROM node:16-alpine3.14 AS build

RUN apk add curl
WORKDIR /usr/src/app
COPY package.json ./
RUN yarn install --production --pure-lockfile
COPY ./ ./

CMD [ "yarn", "start" ]
