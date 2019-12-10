FROM node:10

MAINTAINER Emmanuel Ibe <emmanuel@audioplug.co

# Create app directory
WORKDIR /backwood/src/newsletterdesigner

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN yarn install
# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 301
CMD [ "yarn", "start" ]
