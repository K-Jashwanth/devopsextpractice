
# Use Node.js base image
FROM node:22-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install 

# Copy backend application
COPY dockercont/server.js ./server.js

# Expose application port
EXPOSE 5000

# Start backend server
CMD ["node", "server.js"]
