FROM ubuntu:12.04
MAINTAINER Jeffrey4l <zhang.lei.fly@gmail.com>

ENV HOME /root

COPY sources.list /etc/apt/sources.list

RUN rm -rf /etc/apt/sources.list.d/* && \
    apt-get update && \
    apt-get install -y apt-utils && \
    apt-get install -y python-pip && \
    apt-get install -y tmux

RUN mkdir -p /data

CMD ["/bin/bash"]
