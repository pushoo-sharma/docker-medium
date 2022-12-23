FROM node:lts-alpine
# ENV NODE_ENV=production
WORKDIR /app
COPY ["package.json", "package-lock.json*", "npm-shrinkwrap.json*", "./"]
RUN npm install --silent && mv node_modules ../
COPY . .
EXPOSE 4000
RUN chown -R node /app
USER node
CMD ["npm", "start"]
