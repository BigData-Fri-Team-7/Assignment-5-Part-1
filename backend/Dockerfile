# Use an official Python runtime as a parent image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the requirements file and install dependencies
COPY requirements.txt .
RUN pip install --upgrade pip && pip install -r requirements.txt

# Copy the rest of the backend code into the container
COPY . .

# Expose the port that your FastAPI app will use (8000 is used in our example)
EXPOSE 8000

# Command to run the FastAPI application using uvicorn.
# Here we choose the file that is intended as the entry point.
CMD ["uvicorn", "backend.web_search_agent:app", "--host", "0.0.0.0", "--port", "8000"]
