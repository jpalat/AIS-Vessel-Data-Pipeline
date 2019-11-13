FROM python:3
LABEL maintainer "Jay Palat <vpalat@sei.cmu.edu>"

ENV http_proxy "http://proxy.sei.cmu.edu:8080"
ENV https_proxy "http://proxy.sei.cmu.edu:8080"
ENV HTTP_PROXY "http://proxy.sei.cmu.edu:8080"
ENV HTTPS_PROXY "http://proxy.sei.cmu.edu:8080"
ENV LOCALCLASSPATH "/app"

ENV LANG C.UTF-8

EXPOSE 8888


RUN pip3 install pipenv
COPY requirements.txt /tmp

RUN pip3 install -r /tmp/requirements.txt

COPY . /app

