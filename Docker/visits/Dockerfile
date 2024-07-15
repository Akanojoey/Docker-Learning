FROM node:18-alpine3.20

WORKDIR "/app-test"

COPY package.json .

RUN npm install

COPY . .

CMD ["npm", "start"]
