FROM mcr.microsoft.com/devcontainers/java:17

# Ensure JAVA_HOME is set correctly and available
ENV JAVA_HOME=/usr/lib/jvm/msopenjdk-current
ENV PATH=$JAVA_HOME/bin:$PATH

# Install Gradle (if not already included)
RUN apt-get update && apt-get install -y gradle && rm -rf /var/lib/apt/lists/*

# Verify Java installation
RUN java -version && echo "JAVA_HOME=$JAVA_HOME" && ls -la $JAVA_HOME

# Set working directory
WORKDIR /workspace