FROM ubuntu:12.04
MAINTAINER Jeffrey4l <zhang.lei.fly@gmail.com>

ENV HOME /root
# http://stackoverflow.com/questions/22466255/is-it-possibe-to-answer-dialog-questions-when-installing-under-docker
ENV DEBIAN_FRONTEND noninteractive

COPY sources.list /etc/apt/sources.list

RUN rm -rf /etc/apt/sources.list.d/* && \
    apt-get update && \
    apt-get install -y apt-utils && \
    apt-get install -y python-pip && \
    apt-get install -y tmux && \
    apt-get install -y vim

RUN mkdir -p /data

CMD ["/bin/bash"]
