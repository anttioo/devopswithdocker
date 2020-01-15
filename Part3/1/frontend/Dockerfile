FROM node:10
WORKDIR /usr/src/frontend-example
COPY . .
RUN npm install
RUN npm update
ENV API_URL http://192.168.99.103/api
CMD npm start
EXPOSE 5000