# Use a small Python base image
FROM python:3.12-alpine

# Set working directory
WORKDIR /app

# Create a simple Python script inside container
COPY <<EOF hello.py
print("Hello from Python in Docker!")
EOF

# Default command to run the script
CMD ["python", "hello.py"]
