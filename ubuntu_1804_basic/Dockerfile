FROM ubuntu:18.04
MAINTAINER Jinwon Pyo gch99517@gmail.com

RUN sed -i 's@archive.ubuntu.com@kr.archive.ubuntu.com@g' /etc/apt/sources.list

RUN apt-get update
RUN apt-get install -y build-essential
RUN apt-get install -y cmake
RUN apt-get install -y vim
RUN apt-get install -y net-tools
RUN apt-get install -y git
RUN git config --global alias.co checkout
RUN git config --global alias.br branch
RUN git config --global alias.ci commit
RUN git config --global alias.st status