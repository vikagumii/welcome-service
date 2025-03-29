# Use Python 3.6 as the base image
FROM python:3.6

# Set the working directory to /app
WORKDIR /app

# Copy the requirements file and install dependencies
COPY requirements.txt /app
RUN pip install -r requirements.txt

# Copy the API code into the container
COPY back.py /app

# Expose port 3000
EXPOSE 3000

# Command to run the application
CMD ["python", "back.py"]