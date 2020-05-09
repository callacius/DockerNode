FROM ubuntu:20.04
MAINTAINER Daniel Costa <callacius@gmail.com>

RUN apt update -y\
 && apt upgrade -y\
 && apt install -y --force-yes --no-install-recommends\
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