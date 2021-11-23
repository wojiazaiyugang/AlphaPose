FROM pytorch/pytorch:1.4-cuda10.1-cudnn7-devel

ENV PATH=/usr/local/cuda/bin/:$PATH
ENV LD_LIBRARY_PATH=/usr/local/cuda/lib64/:$LD_LIBRARY_PATH

RUN apt-get update && \
    apt-get -y install libyaml-dev cmake vim libsm6 libxrender1 libxext-dev libgl1-mesa-glx libglib2.0-dev
# pip版本要固定，pip 21.3以后有个不兼容的更新
RUN pip install pqi && pqi use aliyun && pip install pip==21.2.4 && pip install cython pudb opencv-python cython_bbox