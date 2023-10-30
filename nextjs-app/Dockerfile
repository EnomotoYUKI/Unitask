
# Use the official Node.js base image
FROM node:20.5.0

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json for dependency installation
COPY package*.json ./

# Install Node.js dependencies
RUN npm install

# Copy the Next.js application code into the container
COPY . .

# Expose port 3000 for the Next.js application
EXPOSE 3000

# Start the Next.js application
CMD ["npm", "run" , "dev"]
