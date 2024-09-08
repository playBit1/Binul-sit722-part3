# Use Python as the base image
FROM python:latest

# Set the working directory
WORKDIR /app

# Copy the requirements file
COPY requirements.txt .

# Install the required packages
RUN pip install -r requirements.txt

# Copy the application code
COPY . .

# Set environment variables for DB
ENV DATABASE_URL=postgresql://task3db_user:TIvl0maLWmIkSItDX61dwXNn5KdGV5Ld@dpg-cregf9jv2p9s73cv1ju0-a.singapore-postgres.render.com/task3db

# Run the application
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8001"]




