from node:7.4-alpine

maintainer James Kyburz "james.kyburz@gmail.com"

ONBUILD WORKDIR /usr/src/app
ONBUILD ADD package.json /usr/src/app/
ONBUILD RUN npm install
ONBUILD ADD . /usr/src/app
ONBUILD CMD npm start
