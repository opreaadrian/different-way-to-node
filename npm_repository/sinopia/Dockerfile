FROM ubuntu:trusty
MAINTAINER Adrian Oprea<adrian@codesi.nz>

ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update
RUN apt-get install -qy curl build-essential python
RUN curl -sL https://deb.nodesource.com/setup_0.12 | sudo bash -
RUN apt-get install -y nodejs
RUN npm i -g sinopia
RUN adduser --disabled-password --gecos "" sinopia
EXPOSE 4873
ENTRYPOINT ["sinopia"]
