FROM node

WORKDIR /app

COPY package.json /app/

RUN npm i

# If using bind mounts absolute_pathname/:app:ro
# You don't need to copy
# COPY . .

EXPOSE 80

# VOLUME ["/app/node_modules"]

CMD ["npm", "start"]