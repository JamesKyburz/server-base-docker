from node:7.9-alpine

maintainer James Kyburz "james.kyburz@gmail.com"

ONBUILD WORKDIR /usr/src/app
ONBUILD ADD package.json /usr/src/app/
ONBUILD RUN apk --no-cache add --virtual native-deps \
  g++ gcc libgcc libstdc++ linux-headers make python && \
  npm install --quiet node-gyp -g &&\
  npm install --quiet && \
  apk del native-deps
ONBUILD ADD . /usr/src/app
ONBUILD CMD npm start
