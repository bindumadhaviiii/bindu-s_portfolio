# Use the latest Caddy image as the base
FROM caddy:latest

# Set the working directory inside the container
WORKDIR /usr/share/caddy

# Copy the website files to the working directory
COPY . .

# Expose port 80 for HTTP traffic
EXPOSE 80

# Start Caddy with the configuration to serve the current directory
CMD ["caddy", "file-server", "--root", "/usr/share/caddy"]