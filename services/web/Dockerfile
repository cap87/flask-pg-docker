#PULL OFFICIAL IMAGE
FROM python:3.10.6-slim-buster

#Set working directory
WORKDIR /usr/src/app

#Set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

#Install dependencies
RUN pip install --upgrade pip
COPY ./requirements.txt /usr/src/app/requirements.txt
RUN pip install -r requirements.txt

#Copy project
COPY . /usr/src/app/