# Copyright (c) 2019, NVIDIA Corporation. All rights reserved.
#
# This work is made available under the Nvidia Source Code License-NC.
# To view a copy of this license, visit
# https://nvlabs.github.io/stylegan2/license.html

FROM tensorflow/tensorflow:1.15.0-gpu-py3

RUN apt-get update
RUN apt-get install git -y

RUN pip install scipy==1.3.3
RUN pip install requests==2.22.0
RUN pip install Pillow==6.2.1
RUN mkdir /model &&cd $_ && git clone https://github.com/GuillaumeAI/gia-stylegan2.git .

RUN apt-get install vim -y

RUN pip install lmdb
RUN pip install opencv-contrib-python

WORKDIR /model

