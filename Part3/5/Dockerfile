FROM node:10-alpine AS build
WORKDIR /usr/src/frontend-example
COPY . .
ENV API_URL http://192.168.99.103/api
RUN npm install && npm run build


FROM node:10-alpine
WORKDIR /usr/src/frontend-example
COPY --from=build /usr/src/frontend-example/ /usr/src/frontend-example
RUN npm install -g serve
ENV API_URL http://192.168.99.103/api
USER node
CMD serve -s -l 5000 dist
EXPOSE 5000