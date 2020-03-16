FROM node:10

WORKDIR /front-end

COPY package*.json ./

RUN npm ci

COPY . . 

RUN npm run start

EXPOSE 3002

CMD [ "node", "server.js" ]