FROM node:16-alpine

RUN mkdir -p /app

WORKDIR /app

COPY package.json /app/
COPY package-lock.json /app/

RUN npm ci

COPY . /app/

CMD [ "npm", "start" ]