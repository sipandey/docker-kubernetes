# Specify a base image
FROM node:alpine

# Specifying the working directory
WORKDIR /usr/app

# Copy only package.json so that it does not unnecessarily builds again and again
COPY ./package.json ./

# Install some dependencies
RUN npm install

# Copying rest of the files
COPY ./ ./

# Default command
CMD ["npm", "start"]