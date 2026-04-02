FROM node:20
WORKDIR /app
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/users" \
    REDIS_URL="redis://redis:6379"
RUN npm install
COPY package.json .
COPY server.js . 
CMD ["node","server.js"]