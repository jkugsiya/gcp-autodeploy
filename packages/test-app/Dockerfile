FROM node:slim

WORKDIR /app

COPY . /app

RUN npm i --include=dev

RUN cd /app/packages/test-app && npm run build

ENTRYPOINT cd /app/packages/test-app && npm start
