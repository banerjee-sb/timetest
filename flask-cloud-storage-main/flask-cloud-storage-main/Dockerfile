# Dockerfile
FROM python:alpine3.7
COPY requirements.txt /
RUN pip3 install -r /requirements.txt
COPY app.py .
CMD ["gunicorn" , "-b", "127.0.0.1:8080", "app:app"]
