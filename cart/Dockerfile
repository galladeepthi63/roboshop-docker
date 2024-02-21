#reduce the image size 18.19.1-alpine3.19
FROM node:18.19.1-alpine3.19    
EXPOSE 8080
# run below user from root 
RUN addgroup -S roboshop && -S roboshop -G roboshop
WORKDIR /opt/server
ENV MONGO=true
RUN chown roboshop:roboshop /opt/server
USER roboshop
COPY package.json /opt/server/
COPY server.js /opt/server/ 
RUN npm install
CMD ["node", "server.js"]