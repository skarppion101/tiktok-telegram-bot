FROM node:20.10

# Create and define the node_modules's cache directory.
WORKDIR /cache

# install app dependencies
COPY package.json .
COPY package-lock.json .

RUN npm install -g nodemon
RUN npm i

WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH
COPY . .
