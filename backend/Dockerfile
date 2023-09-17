# Dockerfile

# pull the official docker image
FROM python:3.11

# set work directory
WORKDIR /api-app

# set env variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .

RUN apt-get update && apt-get install -y nginx


COPY ./nginx/default.conf /etc/nginx/nginx.conf
