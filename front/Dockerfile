# Use Python 3.6 as the base image
FROM python:3.6

# Set the working directory to /app
WORKDIR /app

# Copy the application files into the container
COPY . /app

# Install dependencies
RUN pip install -r requirements.txt

# Expose port 3001
EXPOSE 3001

# Command to run the application
CMD ["python", "front.py"]