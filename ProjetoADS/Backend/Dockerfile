FROM node:22

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY APP ./APP

# Expose the port the app runs on
EXPOSE 3000

# Command to run the application
CMD ["node", "APP/app.js"]