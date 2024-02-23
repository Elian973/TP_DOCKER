FROM node:20-alpine
WORKDIR /app

COPY ./src ./
RUN npm install

CMD ["node","server.js"]
EXPOSE 3000