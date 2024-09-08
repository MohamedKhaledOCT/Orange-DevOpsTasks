# Base image: node
FROM node:14

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json ./
RUN npm install

# Copy the entire React app
COPY . .

# Build the React app for production
RUN npm run build

# Expose port 3000
EXPOSE 3000

# Start the React app
CMD ["npm", "start"]
