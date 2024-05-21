FROM node:22.2.0-alpine3.19

ENV NODE_ENV=production

WORKDIR /app

COPY package*.json /app/

RUN npm ci

RUN npm install pm2@latest -g

COPY . /app
