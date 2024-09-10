FROM node:alpine

WORKDIR /app

EXPOSE 300

COPY package*.json ./

RUN npm install

COPY . .

RUN chown -R node /app/node_modules

CMD [ "npm", "run", "dev" ]