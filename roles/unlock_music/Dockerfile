# Dockerfile for building the unlock-music web package

FROM node:17-alpine

WORKDIR /app

# https://stackoverflow.com/questions/69692842/error-message-error0308010cdigital-envelope-routinesunsupported
ENV NODE_OPTIONS=--openssl-legacy-provider

EXPOSE 8080

COPY . .

RUN npm i -g http-server

RUN npm install

RUN npm run build

RUN rm -rf ./node_modules

CMD http-server ./dist -p 8080
