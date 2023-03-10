FROM node:16-alpine

WORKDIR /usr/app

COPY ./package.json .

RUN yarn install

COPY . .

ENV BACKEND_PORT=8000

ENV NODE_ENV production

RUN yarn build

CMD [ "yarn", "start" ]

EXPOSE 3000