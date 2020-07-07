FROM node:12
            
USER root
ADD . /usr/src/app
WORKDIR "/usr/src/app"

RUN npm install
