FROM ubuntu:latest
MAINTAINER Mustafa İsmail TÜRKOĞLU <1996mit@gmail.com>
RUN apt update \
  && apt install -y python-pip \
  && apt install -y git
RUN mkdir helloworld
COPY . /helloworld
WORKDIR /helloworld
RUN git clone https://github.com/Sysnove/flask-hello-world.git .
RUN pip install -r requirements.txt
CMD python hello.py
EXPOSE 8000