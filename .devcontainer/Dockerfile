FROM mcr.microsoft.com/devcontainers/java:17

# Install additional tools for Kafka development
RUN apt-get update && apt-get install -y \
    gradle \
    scala \
    && rm -rf /var/lib/apt/lists/*

# Set JAVA_HOME (usually already set in the base image)
ENV JAVA_HOME=/usr/lib/jvm/msopenjdk-current

# Set working directory
WORKDIR /workspace

# Ensure gradle wrapper is executable (will be done when repo is cloned)
# RUN chmod +x gradlew