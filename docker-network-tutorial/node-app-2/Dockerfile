FROM node:alpine

WORKDIR /usr/docker-node-app2

COPY package.json .

RUN npm install

COPY . .

CMD [ "npm", "start" ]