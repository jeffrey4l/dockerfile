FROM jeffrey4l/ubuntu:12.04
MAINTAINER Jeffrey4l <zhang.lei.fly@gmail.com>

RUN apt-get install -y build-essential python-dev && \
        pip install uwsgi && \
        apt-get purge -y build-essential python-dev && \
        rm -rf /tmp/pip* && \
        rm -rf /var/lib/apt/lists/*  && \
        mkdir -p /data/uwsgi

CMD uwsgi --socket 0.0.0.0:9001 -M -

