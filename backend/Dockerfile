FROM node:14-alpine3.16 AS build

RUN npm install pm2

WORKDIR /src

COPY . .

RUN npm install

# RUN npm run build

# CMD ["npm", "run", "start:production"]

CMD ["npm", "run", "start"]

EXPOSE 3000
