VERSION 0.8
FROM python:3
WORKDIR /app

build:
     # In Python, there's nothing to build.
     COPY requirements.txt .
     RUN pip install -r requirements.txt
     
     # Copy application files
     COPY . .

docker:
    SAVE IMAGE flask-calculator:latest

    CMD ["python", "app.py"]
