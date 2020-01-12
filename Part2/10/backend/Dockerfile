FROM node:10
WORKDIR /usr/src/backend-example
COPY . .
RUN npm install
ENV FRONT_URL http://192.168.99.103
CMD npm start
EXPOSE 8000