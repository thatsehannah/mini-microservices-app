FROM node:alpine

# fixes the create react app bug to run in docker
ENV CI=true

WORKDIR /app
COPY package.json ./
RUN npm install
COPY ./ ./

CMD ["npm", "start"]