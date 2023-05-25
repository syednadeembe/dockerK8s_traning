FROM python:3.9

WORKDIR /app

RUN pip install --no-cache-dir Flask==2.0.0

COPY server.py .

CMD ["python", "server.py"]
