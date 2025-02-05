FROM node:23-alpine

WORKDIR /app

RUN apk add bash curl wget

RUN npm install

RUN npm run build

RUN npm install -g serve

EXPOSE 8080

CMD ["serve", "-s", "build", "-l", "8080"]
