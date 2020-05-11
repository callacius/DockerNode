FROM callacius/node:base-ubuntu20.04
MAINTAINER Daniel Costa <callacius@gmail.com>

RUN apt-get update  -y\
 && apt-get upgrade -y --force-yes \
 && rm -rf /var/lib/apt/lists/*;

RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -

RUN apt-get install -y nodejs

RUN apt-get install gcc g++ make

RUN curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - \
    echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
    
RUN apt-get update -y\
 && apt-get install -y yarn

ENV NODE_ENV production
WORKDIR /usr/src/app
CMD ["npm","start"]