# Stage 1: Build the React application
FROM node:18-alpine AS build

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and yarn.lock to the working directory
#COPY package*.json yarn.lock ./

COPY . .

# Install dependencies
RUN yarn install

RUN yarn build
# Copy the rest of the application code to the working directory
#COPY . .

# Build the React application
#RUN yarn build

CMD ["yarn", "start"]
