FROM ubuntu:20.04

RUN apt-get update

RUN apt-get install --yes curl

WORKDIR /usr/src/app

COPY ./curlWebsite.sh ./

ENTRYPOINT [ "./curlWebsite.sh" ]

CMD [ "helsinki.fi" ]
