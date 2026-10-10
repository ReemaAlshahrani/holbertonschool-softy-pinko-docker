# Use the latest Nginx image
FROM nginx:latest

# Copy frontend static files to Nginx web directory
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy Nginx configuration file to default.conf location
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
