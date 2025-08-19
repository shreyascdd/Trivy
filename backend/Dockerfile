# Use a small Python base image
FROM python:3.12-alpine

# Set working directory
WORKDIR /app

# Install a known vulnerable Python package
# Flask 0.5 has multiple CVEs
RUN pip install Flask==0.5

# Create a simple Python script inside container
COPY <<EOF hello.py
import flask

print("Hello from Python in Docker with a vulnerable Flask package!")
EOF

# Default command to run the script
CMD ["python", "hello.py"]
