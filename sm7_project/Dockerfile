FROM python:3.8.0

ENV PYTHONUNBUFFERED 1

RUN apt-get -y update
RUN apt-get -y install vim

RUN mkdir /srv/sm7-server
ADD . /srv/sm7-server

WORKDIR /srv/sm7-server

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# EXPOSE 80 8001 8000