FROM jenkins/jenkins:lts

# Switch to root user to install dependencies
USER root

# Ensure package lists are updated and dependencies are installed properly
RUN apt-get update && apt-get install -y --no-install-recommends \
    apt-transport-https \
    ca-certificates \
    make \
    g++ \
    && rm -rf /var/lib/apt/lists/*  # Clean up to reduce image size

# Switch back to the Jenkins user (best practice)
USER jenkins
