# Use Node v14 as the base image.
FROM node:14

# Add everything in the current directory to our image, in the 'app' folder.
ADD . /app

# Install dependencies
RUN cd /app; \
    npm install --production

# Expose our server port.
EXPOSE 8123

# Run our app.
CMD ["node", "/app/index.js"]