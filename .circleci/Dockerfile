FROM floopcz/tensorflow_cc:ubuntu-shared-cuda:0.0.1

RUN wget https://apt.repos.intel.com/intel-gpg-keys/GPG-PUB-KEY-INTEL-SW-PRODUCTS-2019.PUB && apt-key add GPG-PUB-KEY-INTEL-SW-PRODUCTS-2019.PUB && sh -c 'echo deb https://apt.repos.intel.com/mkl all main > /etc/apt/sources.list.d/intel-mkl.list' && apt-get update && apt-get install -y intel-mkl-64bit-2018.2-046
RUN apt-get install -y clang-6.0 ninja-build python3-pip nvidia-opencl-dev libopenblas-dev libboost-dev nvidia-cuda-dev nvidia-cuda-toolkit libgtest-dev libprotobuf-dev git ssh tar gzip ca-certificates sudo
RUN pip3 install meson
RUN ln -s /usr/include/ /usr/include/openblas
