FROM ubuntu:focal

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update -qq
RUN apt-get upgrade -qq
RUN apt-get install python3 -qq
RUN apt-get install python3-pip -qq

COPY requirements.txt /tmp/pip-reqs/
RUN pip3 --disable-pip-version-check --no-cache-dir install -r /tmp/pip-reqs/requirements.txt
