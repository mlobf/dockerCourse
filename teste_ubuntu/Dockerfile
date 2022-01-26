FROM ubuntu:18.04

WORKDIR /app

COPY . .

#RUN add-repository ppa:deadsnakes/ppa

# RUN python3 --version
RUN apt-get update && apt-get install -y python3 python3-pip libpq-dev cmake
RUN pip3 install -r  requirements.txt

