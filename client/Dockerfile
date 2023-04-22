FROM node:bullseye-slim
LABEL maintainer="bensongathu23@gmail.com"
WORKDIR /MyApp
COPY ./package.json /MyApp/package.json
RUN npm install
COPY . /MyApp/

EXPOSE 3000 

CMD [ "npm", "start"]