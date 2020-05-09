FROM ubuntu:focal
MAINTAINER Daniel Costa <callacius@gmail.com>

RUN apt-get update -y\
 && apt-get upgrade -y\
 && apt-get install -y --no-install-recommends\
      apt-transport-https \
      ssh-client \
      build-essential \
      curl \
      ca-certificates \
      git \
      libicu-dev \
      'libicu[0-9][0-9].*' \
      lsb-release \
      python-all \
      rlwrap \
 && rm -rf /var/lib/apt/lists/*;