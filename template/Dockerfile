FROM node:12.21.0-alpine

ENV NODE_ENV production

WORKDIR /usr/app

USER node

COPY --chown=node:node ./dist package*.json ./

RUN npm i --production

CMD ["node", "index.js"]