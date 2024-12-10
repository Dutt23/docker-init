FROM node

WORKDIR /app

COPY package.json /app

RUN npm i

COPY . /app

EXPOSE 80

ENV MONGO_DB_USER_NAME=admin
ENV MONGO_DB_PASSWORD=admin
CMD ["npm", "start"]