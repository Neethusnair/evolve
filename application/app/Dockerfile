FROM node:14.17.0
COPY --chown=node . /home/node/app/ 
USER 1000
WORKDIR /home/node/app/
COPY package.json /home/node/app/
RUN npm install
COPY . /home/node/app/
CMD node app.js
EXPOSE 3000