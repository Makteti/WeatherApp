# Dockerfile
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy requirements file
COPY requirements.txt .

# Install dependencies
RUN pip install -r requirements.txt

# Copy project files (including static folder)
COPY . .

# Set environment variable for Flask
ENV FLASK_APP=app.py

# Expose the port
EXPOSE 5000

# Run the app
CMD ["flask", "run", "--host=0.0.0.0"]
