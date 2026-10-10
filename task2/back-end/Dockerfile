# Use the latest Ubuntu base image
FROM ubuntu:latest

# Update and upgrade APT packages
RUN apt-get update
RUN apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Remove EXTERNALLY-MANAGED restriction to allow pip installation on Ubuntu
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set the working directory inside the container
WORKDIR /app

# Copy api.py into the container's working directory
COPY ./api.py /app/api.py

# Run the Flask application when the container starts
CMD ["python3", "api.py"]
