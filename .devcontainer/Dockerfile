FROM mcr.microsoft.com/devcontainers/java:17

# Install additional tools if needed
RUN apt-get update && apt-get install -y \
    maven \
    gradle \
    && rm -rf /var/lib/apt/lists/*

# Set working directory
WORKDIR /workspace