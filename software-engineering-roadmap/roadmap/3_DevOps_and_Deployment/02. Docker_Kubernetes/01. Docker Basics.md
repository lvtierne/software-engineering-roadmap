# Docker Basics

Docker is a platform that allows you to package applications and their dependencies into containers.

## Key Concepts
- **Containers**: Lightweight, standalone, and executable packages.
- **Images**: Read-only templates used to create containers.
- **Dockerfile**: Script to build Docker images.
- **Docker Compose**: Tool for defining and running multi-container Docker applications.

## Example
```dockerfile
# Dockerfile example for a Node.js application
FROM node:14

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
COPY package*.json ./
RUN npm install

# Bundle app source
COPY . .

EXPOSE 8080
CMD [ "node", "app.js" ]
```

## Learning Resources

- [Docker Official Documentation](https://docs.docker.com/)
- [Docker for Beginners](https://docker-curriculum.com/)

## Next Steps

1. Build and run your own Docker containers.
2. Explore Docker Compose for managing multi-container setups.
