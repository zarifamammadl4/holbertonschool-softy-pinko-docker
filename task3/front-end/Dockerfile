FROM nginx:latest

# Copy static front-end files
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy Nginx config
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000
EXPOSE 9000
