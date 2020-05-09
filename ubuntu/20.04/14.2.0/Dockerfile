FROM callacius/base-ubuntu20.04
MAINTAINER Daniel Costa <callacius@gmail.com>

RUN curl https://deb.nodesource.com/node_14.x/pool/main/n/nodejs/nodejs_14.2.0-1nodesource1~xenial1_amd64.deb > node.deb \
 && dpkg -i node.deb \
 && rm node.deb

ENV NODE_ENV production
WORKDIR /usr/src/app
CMD ["npm","start"]

RUN apt-get update \
 && apt-get upgrade -y --force-yes \
 && rm -rf /var/lib/apt/lists/*;