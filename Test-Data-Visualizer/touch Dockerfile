# Use the official Node.js 16 image as the base
FROM node:16-alpine

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json (for Node.js dependency management)
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy the rest of the application code to the working directory
COPY . .

# Expose the port that your app runs on (for example, port 3000)
EXPOSE 3000

# Command to start the application
CMD ["npm", "start"]
