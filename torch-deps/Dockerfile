FROM nvidia/cuda:8.0-cudnn7-devel-ubuntu16.04
# Install git and sudo
RUN apt-get update \
 && apt-get install -y \
            git \
            sudo \
 && apt-get clean

RUN git clone https://github.com/torch/distro.git /root/torch --recursive \
 && cd /root/torch \
 && bash install-deps \
 && apt-get clean
