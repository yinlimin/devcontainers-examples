FROM python:3.14.0rc1-slim

RUN apt-get update && apt-get install -y \
    git \
    procps \
    && rm -rf /var/lib/apt/lists/*

RUN pip install flask

COPY . /app
WORKDIR /app

CMD ["python", "app.py"]
