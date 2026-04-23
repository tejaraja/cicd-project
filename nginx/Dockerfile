# Use a lightweight version of the official Nginx image
FROM nginx:stable-alpine

# Remove the default Nginx configuration
RUN rm /etc/nginx/conf.d/default.conf

# Copy your custom configuration into the image
# This assumes the Dockerfile is in the same folder as nginx.conf
COPY nginx.conf /etc/nginx/nginx.conf

# Expose port 80 for incoming traffic
EXPOSE 80

# Start Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]
