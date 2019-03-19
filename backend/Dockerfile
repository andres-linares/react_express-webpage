FROM node:8.15.1-jessie

RUN mkdir -p /srv/app
WORKDIR /srv/app

COPY package.json /srv/app
COPY package-lock.json /srv/app

RUN NPM INSTALL

COPY . /srv/app

CMD ["npm", "run", "start"]