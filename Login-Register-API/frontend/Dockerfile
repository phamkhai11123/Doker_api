# Use Node.js as the base image
FROM node:16-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json (no need for yarn.lock)
COPY package.json ./

# Install dependencies using npm (use `npm install` if you're using npm)
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port the app runs on
EXPOSE 8080

# Command to start the Vue.js development server
CMD ["npm", "run", "dev"]
