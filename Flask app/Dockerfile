# Base image
FROM python:3.9

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file
COPY requirements.txt .

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the application code
COPY . .

# Expose the port the Flask app runs on
EXPOSE 5000

# Run the Flask application
CMD ["python", "app.py"]
