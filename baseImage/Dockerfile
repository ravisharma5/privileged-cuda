# Sample Dockerfile
# FROM ghcr.io/redhat-na-ssa/udi-cuda:11.8.0-cudnn8-devel-ubi8

FROM docker.io/nvidia/cuda:11.8.0-cudnn8-devel-ubi8

USER root

# ENV https_proxy=http://proxy.ebiz.verizon.com:80 \

#    http_proxy=http://proxy.ebiz.verizon.com:80 \

#    no_proxy=.verizon.com,oneartifactoryci.verizon.com,localhost,metadata.google.internal



RUN dnf -y update && \

    dnf -y install sudo && \

    dnf -y install python3.9 && \

    /bin/python3.9 -m pip install ipykernel -U --user --force-reinstall && \X

    pip3 install tensorflow nvidia-cudnn-cu12
