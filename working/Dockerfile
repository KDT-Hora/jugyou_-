FROM ubuntu:latest

RUN apt-get update && apt-get install -y vim locales \
  && rm -rf /var/lib/apt/lists/*
RUN sed -i 's/# ja_JP.UTF-8 UTF-8/ja_JP.UTF-8 UTF-8/' /etc/locale.gen && locale-gen
ENV LANG ja_JP.UTF-8
ENV LC_ALL ja_JP.UTF-8
ENV TZ Asia/Tokyo
