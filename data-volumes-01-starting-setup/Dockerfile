FROM node

WORKDIR /app

COPY package.json /app/

RUN npm i

# If using bind mounts absolute_pathname/:app:ro
# You don't need to copy
# COPY . .

# Changing these changes the layer
# and re-runs everything below it.
ARG DEFAULT_PORT=80

ENV PORT=$DEFAULT_PORT

EXPOSE $PORT

# VOLUME ["/app/node_modules"]

# ARGS cannot be used on this line
# As ARGS are for build time stuff.
# And this is a run time argument
CMD ["npm", "start"]