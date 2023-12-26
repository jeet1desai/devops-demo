# Use the official Ubuntu 20.04 LTS image
FROM ubuntu:latest

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Update package lists and install Python and pip
RUN apt-get update && \
    apt-get install -y python3 python3-pip

# Run app.py when the container launches
CMD ["python3", "test.py"]
