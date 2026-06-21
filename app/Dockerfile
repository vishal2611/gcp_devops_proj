# Use lightweight Nginx base image
FROM nginx:alpine

# Copy the application HTML file to Nginx web root
COPY index.html /usr/share/nginx/html/index.html

# Change Nginx listening port from 80 to 8080
RUN sed -i 's/listen 80;/listen 8080;/g' /etc/nginx/conf.d/default.conf

# Expose port 8080
EXPOSE 8080

# Start Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]


