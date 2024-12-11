FROM node:14-alpine3.16

RUN npm install pm2

WORKDIR /src

COPY . .

RUN npm install

CMD ["npm", "run", "start"]

EXPOSE 3001
