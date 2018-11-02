ARG http_port=3000
FROM node:8

# Create app directory
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install

# for production
# RUN npm install --only=production

# Bundle app source. basically just copying over core app files.
COPY . .

EXPOSE ${http_port}

CMD ["npm", "start"]
