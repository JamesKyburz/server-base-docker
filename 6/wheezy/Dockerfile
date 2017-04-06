from node:6.10-wheezy

maintainer James Kyburz "james.kyburz@gmail.com"

ONBUILD WORKDIR /usr/src/app
ONBUILD ADD package.json /usr/src/app/package.json
ONBUILD RUN npm install
ONBUILD ADD . /usr/src/app
ONBUILD CMD npm start
