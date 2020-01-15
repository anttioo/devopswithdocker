FROM node:10-alpine
WORKDIR /usr/src/frontend-example
COPY . .
RUN npm install
ENV API_URL http://192.168.99.103/api
USER node
CMD npm start
EXPOSE 5000