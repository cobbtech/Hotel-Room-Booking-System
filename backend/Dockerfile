# Use the official Node.js image as the base image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json files to the working directory
COPY . .

# Install dependencies
RUN yarn install

# Copy the rest of the application code to the working directory
#COPY . .

# Expose port 3000 for the Node.js application
EXPOSE 3000

# Command to run the application
CMD ["yarn", "start"]
