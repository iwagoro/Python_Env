FROM python:3.13.0a4-bullseye

ENV DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Tokyo

RUN apt-get update && \
    apt-get -y install --reinstall ca-certificates && \
    apt-get -y install software-properties-common && \
    pip install --upgrade pip

RUN mkdir -p /workspace/app
COPY ./ /workspace
