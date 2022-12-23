FROM node:lts-alpine

WORKDIR /client

COPY package*.json /client/

RUN npm install

# copy everything to the client directory
COPY . /client/

EXPOSE 3000

CMD ["npm", "start"]
