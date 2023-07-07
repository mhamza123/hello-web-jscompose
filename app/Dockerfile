FROM node:alpine

WORKDIR /usr/src/app


COPY package*.json ./

# run npm install in our local machine
RUN npm install

# copy the generated modules and all other files to the container
COPY . .

# our app is running on port 5000 within the container, so need to expose it
EXPOSE 3000

# the command that starts our app
CMD ["node", "index.js"]
