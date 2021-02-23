FROM node:14-alpine

#create app directory
WORKDIR /usr/src/app

COPY package*.json ./

RUN npm ci --only=production
# RUN yarn install

COPY . .

EXPOSE 3001
RUN chmod 700 -R /usr/src

CMD [ "npm","start" ]