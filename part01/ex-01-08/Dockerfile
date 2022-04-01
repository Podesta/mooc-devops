FROM ubuntu:20.04

RUN apt update

RUN apt install --yes curl

WORKDIR /usr/src/app

COPY ./curlWebsite.sh ./

CMD ./curlWebsite.sh
