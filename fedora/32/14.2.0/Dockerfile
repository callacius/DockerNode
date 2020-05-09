FROM callacius/node:base-fedora32
MAINTAINER Daniel Costa <callacius@gmail.com>

RUN sudo dnf -y update

RUN sudo curl -sL https://rpm.nodesource.com/setup_14.x | sudo bash -

RUN sudo dnf -y install gcc-c++ make nodejs-14.2.0

ENV NODE_ENV production
WORKDIR /usr/src/app
CMD ["npm","start"]