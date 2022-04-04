FROM node:16

EXPOSE 5000

WORKDIR /usr/src/app

RUN npm install -g serve

COPY ./example-frontend/package* ./

RUN npm install

COPY ./example-frontend/ ./

ENV REACT_APP_BACKEND_URL=http://localhost:8000

RUN npm run build

ENTRYPOINT [ "serve", "-s", "-l", "5000", "build" ]
