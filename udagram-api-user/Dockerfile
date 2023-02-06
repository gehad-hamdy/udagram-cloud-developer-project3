FROM node:12
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies

COPY package*.json ./
RUN npm ci 
# Bundle app source
COPY . .
EXPOSE 8090
CMD [ "npm", "run", "dev" ]