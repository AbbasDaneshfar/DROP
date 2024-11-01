FROM node:14.16.0-alpine3.13

LABEL maintainer="Abbas Daneshfar <daneshfarabbas@gmail.com>"

RUN addgroup app && adduser -S -G app app
USER app

WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . . 

EXPOSE 3001 

CMD ["npm", "start"]
