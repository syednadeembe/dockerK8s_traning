# Use an official Nginx runtime as a parent image
FROM nginx:latest

# Remove the default Nginx configuration file
RUN rm /etc/nginx/conf.d/default.conf

# Copy the custom configuration file to the container
COPY nginx.conf /etc/nginx/conf.d/

# Copy the custom HTML file to the container
COPY index.html /usr/share/nginx/html/

# Expose port 80 for HTTP traffic
EXPOSE 80
