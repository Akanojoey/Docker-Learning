#FROM node:14

#COPY ./ ./

#RUN npm install

#CMD ["npm", "start"]


# Use the official Node.js 21 Alpine base image
FROM node:21-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json (if available) to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose the port the app runs on
#EXPOSE 8080

# Command to run the application
CMD ["npm", "start"]


# Use the official Node.js image as the base image
#FROM node:14

# Set the working directory inside the container
#WORKDIR /app

# Copy package.json and package-lock.json to the working directory
#COPY package*.json ./

# Clear npm cache and install dependencies
#RUN npm cache clean --force && npm install

# Copy the rest of the application code to the working directory
#COPY . .

# Start the application
#CMD ["npm", "start"]

