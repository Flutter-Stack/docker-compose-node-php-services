FROM node:lts-alpine
RUN mkdir -p /usr/src/app
RUN mkdir -p /usr/src/app/public/files
RUN apk update && apk upgrade && apk add --no-cache bash git openssh
WORKDIR /usr/src/app
#RUN npm install -g nodemon
RUN npm config set save=true
RUN npm config set save-exact=true
RUN  cat /root/.npmrc
#RUN  rm -rf node_modules && npm install
#RUN  npm install nodemon
EXPOSE 8081

# https://dev.to/alex_barashkov/using-docker-for-nodejs-in-development-and-production-3cgp
