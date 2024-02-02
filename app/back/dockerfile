# Use an official Python runtime as a parent image
FROM python:3.8

# Set the working directory to /app/back
WORKDIR /app/back

# Copy the current directory contents into the container at /app/back
COPY . /app/back

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 5000 to the outside world
EXPOSE 5000

# Define environment variable
ENV FLASK_APP=app.py
#your_flask_app_file.py

# Command to run on container start
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]
