# Use Python 3.9 as the base image
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Install the dependencies
COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

# Copy the FastAPI app code
COPY . .

# Expose the port FastAPI will run on
EXPOSE 8000

# Command to start the FastAPI server
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
