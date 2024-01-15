FROM python:3.10.13-slim

WORKDIR /app

COPY ["requirements.txt", "./"]

RUN pip install --upgrade pip && pip install -r requirements.txt

COPY ["app.py", "hospitalization-RFC_model.bin", "./"]

# ENTRYPOINT ["gunicorn", "--workers=8", "--bind", "0.0.0.0:5000", "app:app"]