# Use a compatible Node.js version (16.x)
FROM node:16

# Set the working directory
WORKDIR /app

# Copy package.json and yarn.lock first to install dependencies
COPY package.json yarn.lock ./

# Install dependencies
RUN yarn install --frozen-lockfile

# Copy the rest of your application code
COPY . .

# Expose the application port (if applicable)
EXPOSE 3000

# Start your application (change this command as needed)
CMD ["yarn", "dev"]
