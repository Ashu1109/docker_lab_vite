# Use a base image
FROM node:21-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install -g nodemon typescript
RUN npm install

# Copy the rest of your app
COPY . .

# Expose port (if needed)
EXPOSE 3000

# Start the app
CMD ["npm", "run", "dev"]
