FROM node:19.6.0-alpine
LABEL maintainer="bensongathu23@gmail.com"
WORKDIR /MyApp
COPY ./package.json /MyApp/package.json
RUN npm install
COPY . /MyApp

EXPOSE 5000

CMD [ "npm", "start"]
