FROM node:14

WORKDIR /code

COPY package.json .
COPY package-lock.json .

RUN npm install

CMD ["npm", "run", "serve"]
