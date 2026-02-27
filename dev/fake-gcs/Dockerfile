FROM fsouza/fake-gcs-server@sha256:e7b38a919e3721c1ba02db60d6cd1690ebf03035bfd0a5f989ab70e6c55ab821

# Install curl
RUN apk add --no-cache curl

# Copy the initialization script
COPY start.sh /start.sh
RUN chmod +x /start.sh

# Set the entrypoint
ENTRYPOINT ["/start.sh"]
