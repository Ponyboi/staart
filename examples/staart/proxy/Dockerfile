FROM node:10-jessie

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY package.json package-lock.json ./
RUN npm install

COPY . .

EXPOSE 8080
ENTRYPOINT [ "npm", "run"]
CMD [ "start" ]
