#alpine version of node is very basic level of node
FROM node:alpine

#WORKDIR : if we don't specify this, then all application specific files directly copied
# to container root directory
WORKDIR /usr/app

#COPY : copy everyhting from current workind directory to container
COPY ./package.json ./
RUN npm install
COPY ./ ./



#Install some dependencies
RUN npm install

CMD ["npm","start"]