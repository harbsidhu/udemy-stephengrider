FROM node:alpine

WORKDIR '/usr/visits'

COPY package.json .
RUN npm install
COPY . .

CMD ["npm","start"]