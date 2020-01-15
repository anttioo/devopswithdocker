FROM node:10-alpine
WORKDIR /usr/src/backend-example
COPY .. .
RUN npm install && chown -R node:node /usr/src/backend-example
ENV FRONT_URL http://192.168.99.103
USER node
CMD npm start
EXPOSE 8000