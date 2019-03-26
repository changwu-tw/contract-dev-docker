FROM node:carbon-alpine

RUN apk add -t .gyp --no-cache git python make g++ vim  \
    && npm install -g truffle \
    && apk del .gyp

RUN mkdir -p /workspace
WORKDIR /workspace

EXPOSE 8080
ENTRYPOINT []