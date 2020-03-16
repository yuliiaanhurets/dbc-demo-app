FROM node:10-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm ci

COPY . . 
RUN npm run serve

EXPOSE 3003

CMD [ "node", "server.js" ]