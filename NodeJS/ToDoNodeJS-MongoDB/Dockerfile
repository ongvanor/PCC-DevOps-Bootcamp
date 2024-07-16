FROM node:18.12.1-slim

ENV DB_URL="mongodb"
ENV DB_NAME="test" 

COPY . /opt/nodejs-todo-mongodb
WORKDIR /opt/nodejs-todo-mongodb

RUN npm install
RUN npm run build-prod

ENTRYPOINT ["npm", "run", "serve"]
