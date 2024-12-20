# Use the latest Ubuntu image
FROM ubuntu:latest

RUN apt-get update
# Update package list

RUN apt-get upgrade -y
# Upgrade installed packages

RUN apt-get install -y python3 python3-pip
# Install Python3 and pip

RUN pip3 install Flask
# Install Flask

WORKDIR /app
# Set working directory

COPY ./api.py /app/api.py
# Copy application code

EXPOSE 5252
# Expose port for Flask app

CMD ["python3", "api.py"]
# Run the Flask application