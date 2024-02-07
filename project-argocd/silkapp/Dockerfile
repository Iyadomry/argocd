# Use the official Nginx image as the base image
FROM nginx:latest

# Remove the default nginx.html file
RUN rm /usr/share/nginx/html/index.html

# Copy the custom HTML file into the container
COPY silkapp-content/index.html /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start Nginx and keep it running in the foreground
CMD ["nginx", "-g", "daemon off;"]
