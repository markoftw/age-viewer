FROM node:14-alpine3.16 AS build

RUN npm install pm2

WORKDIR /src

COPY . .

RUN npm install

RUN npm run build

FROM nginx:alpine AS runner

COPY --from=build /src/build /usr/share/nginx/html

EXPOSE 80
