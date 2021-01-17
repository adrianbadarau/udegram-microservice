# latest LTS (long term support) version 12 of node available from the Docker hub
FROM node:12
# Create app directory
WORKDIR /usr/src/app
# Bundle app source
COPY . .
RUN npm install
# If you are building your code for production
# RUN npm ci --only=production
EXPOSE 4200
CMD [ "npm", "start" ]
