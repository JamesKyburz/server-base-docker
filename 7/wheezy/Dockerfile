from node:7.9-wheezy

maintainer James Kyburz "james.kyburz@gmail.com"

ONBUILD WORKDIR /usr/src/app
ONBUILD ADD package.json /usr/src/app/package.json
ONBUILD RUN npm install --quiet
ONBUILD ADD . /usr/src/app
ONBUILD CMD npm start
