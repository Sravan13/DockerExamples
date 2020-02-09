#alpine version of node is very basic level of node
FROM node:alpine

#copy everyhting from current workind directory to container
COPY ./ ./

#Install some dependencies
RUN npm install

CMD ["npm","start"]