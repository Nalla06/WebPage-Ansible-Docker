FROM node:14

# Create app directory
WORKDIR /usr/src/app


COPY package*.json ./

RUN npm install
# If we are building our code for production
# RUN npm ci --only=production


# copy all files into the image
COPY . .

EXPOSE 5000

CMD ["node","app.js"]