# Use the official Python image
FROM python:3.12

# Set the working directory
WORKDIR /app

# Copy the project files into the container
COPY .. .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 8000
EXPOSE 8000

# Run migrations and start the Django app
CMD ["sh", "-c", "python manage.py runserver 0.0.0.0:8000"]
