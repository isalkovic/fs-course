FROM mhart/alpine-node:11

CMD mkdir /webme
WORKDIR /webme

COPY server.js .
COPY LICENSE .
COPY package.json .
COPY package-lock.json .
COPY README.md .
COPY LICENSE .
COPY lib ./lib
COPY public ./public

RUN npm install

EXPOSE 4100

CMD ["node", "server.js"]
