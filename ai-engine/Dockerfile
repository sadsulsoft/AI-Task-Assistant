# /ai-engine/Dockerfile

# Use the official Python image
FROM python:3.9-slim

# Set the working directory
WORKDIR /app

# Copy the requirements file and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code
COPY . .

# Expose the port the application runs on
EXPOSE 5000

# Command to run the application (e.g., using gunicorn)
CMD ["gunicorn", "--bind", "0.0.0.0:5000", "app:app"]
