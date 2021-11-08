# syntax=docker/dockerfile:1
FROM node:17-alpine
RUN apk add --no-cache python3 g++ make
RUN apk add --update nodejs npm 
WORKDIR /app
COPY . .
RUN npm install -g npm@8.1.3
RUN npm install --production
CMD ["node", "src/index.js"]
