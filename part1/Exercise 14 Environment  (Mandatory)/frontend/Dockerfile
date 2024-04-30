FROM node:16.0-alpine


COPY package*.json .

RUN npm install

COPY . .

ENV REACT_APP_BACKEND_URL=http://10.10.10.100:8080

EXPOSE 5000

RUN npm run build

RUN npm install -g serve


CMD [ "serve", "-s", "-l", "5000", "build" ]