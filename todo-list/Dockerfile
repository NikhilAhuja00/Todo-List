# pull official base image
FROM node

# set working directory
WORKDIR /app/frontend

#install app dependencies
COPY package*.json ./

RUN npm install

COPY . ./

EXPOSE 3000

CMD ["npm","start"]
