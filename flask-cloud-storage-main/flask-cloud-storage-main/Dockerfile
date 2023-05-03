# Use an official Python runtime as a parent image
FROM python:3.9

 

# Set the working directory to /app
WORKDIR /app

 

# Copy the requirements file into the container
COPY requirements.txt .

 

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

 

# Copy the application code into the container
COPY . .

 

# Expose the port that the app will listen on
EXPOSE 8080

 

# Run the command to start the Flask app
CMD ["python", "main.py"]
