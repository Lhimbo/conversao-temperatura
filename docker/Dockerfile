FROM node:16-alpine

WORKDIR /app

COPY /src/package.json /app
RUN npm install

COPY . /app

EXPOSE 8080
CMD ["node", "server.js"]