FROM node:10-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install -g http-server && npm ci

COPY . . 

RUN npm run build

EXPOSE 8080

CMD [ "http-server", "dist" ]