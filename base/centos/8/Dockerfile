FROM centos:8
MAINTAINER Daniel Costa <callacius@gmail.com>

RUN dnf -y update \ 
 && dnf clean all

RUN dnf install -y \
 https://download1.rpmfusion.org/free/el/rpmfusion-free-release-8.noarch.rpm
  
RUN dnf install -y \
 https://download1.rpmfusion.org/nonfree/el/rpmfusion-nonfree-release-8.noarch.rpm
  
RUN dnf module list nodejs

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
    which \
 && dnf clean all

