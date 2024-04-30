FROM node:16.0-alpine

COPY package*.json .

RUN npm install

COPY . .

EXPOSE 5000

RUN npm run build

RUN npm install -g serve

CMD [ "serve", "-s", "-l", "5000", "build" ]