# Base image for dev containers
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Set environment variables to avoid interactive prompts
ENV DEBIAN_FRONTEND=noninteractive

# Install common dependencies
RUN apt-get update && apt-get install -y \
    curl \
    git \
    unzip \
    gnupg \
    ca-certificates \
    && rm -rf /var/lib/apt/lists/*

# Install Node.js (use LTS version)
RUN curl -fsSL https://deb.nodesource.com/setup_18.x | bash - \
    && apt-get install -y nodejs

# Install Salesforce CLI (sf)
RUN curl -s https://developer.salesforce.com/media/salesforce-cli/install.sh | bash

# Verify installation
RUN sf version

# Optional: Install prettier, eslint, and other global dev tools
RUN npm install -g prettier eslint

# Set bash as default shell
CMD [ "bash" ]
