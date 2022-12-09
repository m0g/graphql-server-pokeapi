FROM node:16

# set working directory
WORKDIR /usr/src/app

#RUN apk add --no-cache git python3 g++ make py3-pip build-base
RUN apt-get update && apt-get install -y build-essential

# install app dependencies
COPY package.json ./
RUN npm install

# add app
COPY . ./

# start app
CMD ["npm", "start"]
