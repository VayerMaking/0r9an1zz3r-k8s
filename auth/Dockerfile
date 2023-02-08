FROM node:17-alpine as builder

WORKDIR /home/api

COPY package*.json ./

RUN npm install

COPY . .
# COPY .env .
RUN chmod +x ./start.sh

EXPOSE 5000

ENTRYPOINT ["./start.sh"]