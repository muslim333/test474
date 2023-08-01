# Use the official Nginx base image
FROM nginx:latest

# (Optional) Copy your custom Nginx configuration file
# COPY nginx.conf /etc/nginx/nginx.conf

# (Optional) Copy any additional static files for your website
# COPY index.html /usr/share/nginx/html/

# (Optional) Copy SSL certificates if you need HTTPS support
# COPY ssl-cert.crt /etc/nginx/ssl/
# COPY ssl-cert.key /etc/nginx/ssl/

# Expose the necessary port(s)
EXPOSE 80
# EXPOSE 443 # Uncomment this line if you are using SSL and want to expose port 443 as well.

# (Optional) Set environment variables (if needed)
# ENV MY_VARIABLE=value

# (Optional) You can add other configurations, like setting up a user, changing permissions, etc.

# Start the Nginx server
CMD ["nginx", "-g", "daemon off;"]
