FROM ubuntu:18.04
LABEL Description="Build environment"

ENV HOME /root

RUN apt-get update && apt-get -y --no-install-recommends install \
    build-essential \
    cmake \
    wget \
    libtbb-dev \
    doxygen \
    libeigen3-dev \
    python3-pip \
    python-pip \
    python3-dev \
    libboost-all-dev \
    vim 
