FROM node:16

EXPOSE 5000

WORKDIR /usr/src/app

RUN npm install -g serve

COPY ./example-frontend/package* ./

RUN npm install

COPY ./example-frontend/ ./

RUN npm run build

ENTRYPOINT [ "serve", "-s", "-l", "5000", "build" ]
