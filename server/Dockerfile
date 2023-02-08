FROM alpine:3.15

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY package.json .

RUN apk add --update nodejs npm

RUN npm install

COPY . .

EXPOSE 8000

CMD ["npm", "start"]