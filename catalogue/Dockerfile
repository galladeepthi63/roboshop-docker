FROM node:18
EXPOSE 8080
WORKDIR /opt/server
ENV MONGO=true
COPY package.json /opt/server/
COPY server.js /opt/server/
# npm install get the dependencies of node js project
RUN npm install
ENTRYPOINT ["node", "server.js"]
