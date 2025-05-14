# Step 1: Use Node.js as the base image
FROM node:16

# Step 2: Set the working directory
WORKDIR /app

# Step 3: Install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Step 4: Copy the server code into the container
COPY . .

# Step 5: Expose the backend port
EXPOSE 5000

# Step 6: Run the application
CMD ["node", "server.js"]

