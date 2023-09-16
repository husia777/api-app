# Dockerfile

# pull the official docker image
FROM python:3.11

COPY . .
WORKDIR /api-app

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

RUN pip install -r requirements.txt
