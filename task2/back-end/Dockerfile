FROM ubuntu:latest

# Update and upgrade system
RUN apt-get update && apt-get upgrade -y

# Install Python and pip
RUN apt-get install -y python3 python3-pip

# Fix "externally managed" pip error if it occurs
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set working directory
WORKDIR /app

# Copy the Flask app
COPY ./api.py /app/api.py

# Expose the port Flask runs on
EXPOSE 5252

# Run the Flask server
CMD ["python3", "api.py"]

