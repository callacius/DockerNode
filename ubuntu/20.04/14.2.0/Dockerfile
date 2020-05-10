FROM callacius/base-ubuntu20.04
MAINTAINER Daniel Costa <callacius@gmail.com>

RUN sudo apt-get update  -y\
 && sudo apt-get upgrade -y --force-yes \
 && rm -rf /var/lib/apt/lists/*;

RUN curl -sL https://deb.nodesource.com/setup_14.x | sudo bash -

RUN sudo apt-get install -y nodejs

RUN sudo apt-get install gcc g++ make

RUN curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - \
    echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
    
RUN sudo apt-get update -y\
 && sudo apt-get install -y yarn

ENV NODE_ENV production
WORKDIR /usr/src/app
CMD ["npm","start"]