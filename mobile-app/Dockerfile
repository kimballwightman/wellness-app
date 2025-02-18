# Use Node.js official image as a base
FROM node:18

# Set working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json from wellnessappmobile folder
COPY wellnessappmobile/package.json wellnessappmobile/package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the project files from wellnessappmobile
COPY wellnessappmobile/ ./

# Expose port for React Native
EXPOSE 19000

# Command to start React Native development server
CMD ["npm", "start"]
