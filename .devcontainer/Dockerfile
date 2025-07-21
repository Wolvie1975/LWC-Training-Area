FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Install Node.js and npm first
RUN apt-get update && apt-get install -y curl ca-certificates gnupg
RUN curl -fsSL https://deb.nodesource.com/setup_18.x | bash -
RUN apt-get install -y nodejs

# Install Salesforce CLI using the official npm package
RUN npm install --global @salesforce/cli

