# Start with Python 3.11 as base
FROM python:3.11-slim

# Set working directory inside container
WORKDIR /app

# Copy requirements first (for caching)
COPY requirements.txt .

# Install dependencies
RUN pip install -r requirements.txt

# Copy your app code
COPY . .

# Expose port 5000
EXPOSE 5000

# Run the app
CMD ["python", "app.py"]
