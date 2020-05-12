FROM callacius/node:base-centos8
MAINTAINER Daniel Costa <callacius@gmail.com>

RUN dnf -y update

RUN curl -sL https://rpm.nodesource.com/setup_14.x | bash -

RUN dnf -y install gcc-c++ make nodejs-14.2.0

ENV NODE_ENV production
WORKDIR /usr/src/app
CMD ["npm","start"]