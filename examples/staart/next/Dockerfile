FROM node:10.15.3

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY package.json package-lock.json ./
RUN npm install

COPY . .
RUN npm run build

ENTRYPOINT [ "npm", "run"]
CMD [ "start" ]
