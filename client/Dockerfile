# Stage 1: build
FROM node:16.16.0 AS development

WORKDIR /client/src/app

COPY package*.json ./

RUN npm install
RUN npm install -g @angular/cli@9.1.0

COPY . .

RUN npm run build

EXPOSE 4200
