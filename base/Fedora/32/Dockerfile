FROM fedora:32

MAINTAINER Daniel Costa <callacius@gmail.com>

RUN dnf -y update && dnf clean all

RUN dnf install -y \
      automake \
      libicu \
      curl \
      gcc \
      gcc-c++ \
      git \
      kernel-devel \
      make \
      perl \
      python \
      which \
 && dnf clean all

