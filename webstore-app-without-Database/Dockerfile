# Use Node.js LTS
FROM node:18-alpine

# Set working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json first
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy the rest of the project files
COPY . .

# Expose the port the app runs on (default Express port)
EXPOSE 3000

# Start the app
CMD ["node", "app.js"]
