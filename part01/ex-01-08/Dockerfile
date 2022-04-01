FROM ubuntu:20.04

RUN apt update

RUN apt install --yes curl

WORKDIR /us/src/app

COPY ./curlWebsite.sh ./

CMD ./curlWebsite.sh
