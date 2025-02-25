# Use an official Python image
FROM python:3.9

# Set the working directory inside the container
WORKDIR /app

# Copy the backend code to the container
COPY . .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Install TensorFlow separately to ensure compatibility
RUN pip install --no-cache-dir tensorflow h5py

# Expose the port your app runs on
EXPOSE 5000

# Command to run the app
CMD ["python", "app.py"]
