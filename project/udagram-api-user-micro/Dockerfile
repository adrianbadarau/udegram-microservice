# specify the node base image with your desired version node:<version>
FROM node:12

# Create app directory
WORKDIR /usr/

ENV POSTGRES_DATABASE postgres
ENV POSTGRES_HOST 172.19.0.2
ENV POSTGRES_PASSWORD mysecretpassword
ENV POSTGRES_USERNAME postgres

COPY package*.json ./
RUN npm install
# Bundle app source
COPY www/. .

EXPOSE 8080
CMD [ "node", "server.js" ]

