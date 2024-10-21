# Dockerfile for Next.js Frontend
FROM node:23.0.0

WORKDIR /app

# Copy package files and install dependencies
COPY ./package*.json ./
RUN npm install

# Copy the rest of the application code
COPY ./app ./app

# Build the Next.js application
RUN npm run build

# Expose the port on which the application runs
EXPOSE 3000

# Start the application
CMD ["npm", "run", "dev"]
