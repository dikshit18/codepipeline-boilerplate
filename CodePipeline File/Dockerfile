#!/bin/bash

FROM node:12.16.1-alpine3.11

WORKDIR /server

COPY package*.json ./

RUN npm ci

COPY . .

RUN ls -shal /server

EXPOSE 3001

CMD ["node", "app.local.js"]