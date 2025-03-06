FROM node:alpine
LABEL maintainer="pedro-henrique-teles"

WORKDIR /home/app

RUN apk add --no-cache bash

COPY package*.json ./

RUN npm i

COPY . .

RUN npm run build

EXPOSE 9001

CMD ["npm", "run", "start:dev"]
