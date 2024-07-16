FROM node:18.12.1-slim

COPY . /opt/nodejs-todo-mysql
WORKDIR /opt/nodejs-todo-mysql

RUN npm install
RUN npm run build-prod

ENTRYPOINT ["npm", "run", "serve"]
