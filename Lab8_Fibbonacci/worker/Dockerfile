FROM node:14.14.0-alpine
WORKDIR "/app"
ENV NODE_OPTIONS=--openssl-legacy-provider
COPY ./package.json ./
RUN npm install
RUN chown -R node:node . /app
CMD ["npm", "run", "dev"]
