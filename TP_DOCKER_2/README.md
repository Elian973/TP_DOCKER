# TP2 DOCKER

## 1 . Récupérer le code source du TP et le mettre dans TP_DOCKER_2

## 2 . Créer un Dockerfile qui permet de lancer une application NodeJS (v20-alpine)

```bash
FROM node:20-alpine
WORKDIR /app

COPY ./src ./
RUN npm install

CMD ["node","server.js"]
EXPOSE 3000
```

## 3 . Utilisez docker pour lancer une image de base de données (mysql)
