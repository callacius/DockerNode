FROM callacius/node:base-fedora32
MAINTAINER Daniel Costa <callacius@gmail.com>

RUN sudo dnf install -y \
  https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm
  
RUN sudo dnf install -y \
  https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
  
RUN sudo dnf -y update

RUN sudo dnf install -y nodejs 

ENV NODE_ENV production
WORKDIR /usr/src/app
CMD ["npm","start"]