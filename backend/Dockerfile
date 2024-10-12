# Start with a base image
FROM node:16

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the app
COPY . .

# Expose the port and start the app
EXPOSE 3000
CMD ["npm", "run", "start:dev"]
