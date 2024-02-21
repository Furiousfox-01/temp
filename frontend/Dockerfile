# Use an official Nginx image as a parent image
FROM nginx:alpine

# Copy the static site files from your machine to the container
COPY . /usr/share/nginx/html

# Copy the Nginx configuration files
COPY nginx.conf /etc/nginx/nginx.conf
COPY default.conf /etc/nginx/conf.d/default.conf

# Expose port   80 for HTTP
EXPOSE   80

# Start Nginx when the container launches
CMD ["nginx", "-g", "daemon off;"]
