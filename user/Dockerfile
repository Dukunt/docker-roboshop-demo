FROM node:20
WORKDIR /app
COPY *.js .
COPY package.json .
ENV MONGO = "true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue" \
    REDIS_URL="redis://redis:6379" 
EXPOSE 8080    
RUN npm install
CMD ["node", "server.js"]     