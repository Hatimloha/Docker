# Flask App

> Follow the below step to craete the flask-app:

## Create the DIR:
```bash
mkdir flask-app
```
## create the file given in repo:
- require files: 
- /flask-app/
  - Dockerfile
  - requirements.txt
  -  app.py

- 1. Dockerfile
```bash
vi Dockerfile
```
```bash
# Use the official Python base image from Docker Hub
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements.txt into the container (optional but recommended)
COPY requirements.txt /app/

# Install dependencies from the requirements.txt file
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application files into the container
COPY . /app/

# Expose the port Flask will run on (default is 5000)
EXPOSE 5000

# Set environment variables (optional for production)
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0

# Run the Flask application
CMD ["flask", "run"]
```
- 2. requirements.txt
```bash
vi requirements.txt
```
```bash
