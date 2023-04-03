FROM ubuntu:bionic

RUN apt-get update && apt-get install -y apt-utils
RUN apt-get install -y python3.6 python3-pip python3.6-dev python3.6-numpy
RUN pip3 install --upgrade pip

ADD . /root/app/server

# Setup server
WORKDIR /root/app/server

RUN python3 -m pip install --upgrade --force pip
RUN pip3 install -r requirements.txt
