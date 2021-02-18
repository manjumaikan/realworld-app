FROM node:10-alpine
WORKDIR /web
COPY . .
RUN apk add --no-cache ca-certificates \
    && apk update \
    && yarn config set "strict-ssl" false -g \
    && yarn global add serve \
    && npm install