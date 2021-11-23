FROM pytorch/pytorch:1.1.0-cuda10.0-cudnn7.5-devel

ENV PATH=/usr/local/cuda/bin/:$PATH
ENV LD_LIBRARY_PATH=/usr/local/cuda/lib64/:$LD_LIBRARY_PATH

RUN apt-get update && apt-get -y install libyaml-dev

RUN pip install pqi && pqi use aliyun && pip install cython