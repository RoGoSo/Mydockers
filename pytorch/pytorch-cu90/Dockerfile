# FROM pytorch/pytorch:1.0-cuda10.0-cudnn7-devel 
FROM nvidia/cuda:9.0-cudnn7-devel-ubuntu16.04
MAINTAINER rengaosheng <iamrgs@foxmail.com>

RUN apt-get update 
RUN apt-get install -y python3-pip
# RUN pip3 install  pytorch torchvision \
RUN conda install -y  numpy \
	scipy \
	scikit-image \
	scikit-learn \
	opencv \
	h5py 
RUN pip install imgaug 

# Set timezone
RUN sudo ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

EXPOSE 8080 