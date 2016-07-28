FROM jenkins
MAINTAINER Zoltan Kornel Torok <taz19880922@gmail.com>
USER root
# ----------------
# Lastest version of NodeJS and NPM
# ----------------
RUN apt-get update
RUN apt-get install -y python-software-properties  
RUN apt-get install -y software-properties-common
RUN apt-get install curl
RUN curl -sL https://deb.nodesource.com/setup_4.x | bash -
RUN apt-get install -y nodejs
# ----------------
# NodeJs dependencies
# ----------------
RUN curl https://install.meteor.com | /bin/sh  
RUN npm install -g chimp 
RUN npm install -g spacejam
RUN npm install -g coffee-script
RUN npm install -g jshint  
RUN npm install -g csslint

USER jenkins
