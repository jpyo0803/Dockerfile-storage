FROM ubuntu:18.04
MAINTAINER Jinwon Pyo gch99517@gmail.com

# change the package serverlist to korea
RUN sed -i 's@archive.ubuntu.com@kr.archive.ubuntu.com@g' /etc/apt/sources.list

# Basic packages to be installed
RUN apt-get update
RUN apt-get install -y build-essential
RUN apt-get install -y cmake
RUN apt-get install -y vim
RUN apt-get install -y net-tools
RUN apt-get install -y git

# Basic git settings
RUN git config --global user.email "gch99517@gmail.com"
RUN git config --global user.name "Jinwon Pyo"
RUN git config --global alias.co checkout
RUN git config --global alias.br branch
RUN git config --global alias.ci commit
RUN git config --global alias.st status

# Prevent CRLF related issue
RUN git config --global core.autocrlf true