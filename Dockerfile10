# from base image node
ARG NODE_VERSION=8.11-slim
FROM node:$NODE_VERSION

LABEL "about"="This file is just am example to demonstarte the LABEL"

ENV workdirectory /usr/node

WORKDIR $workdirectory
WORKDIR app

COPY package.json .

RUN ls -ll &&\
    npm install

ADD index.js .

RUN ls -l

# command executable and version
ENTRYPOINT ["node"]