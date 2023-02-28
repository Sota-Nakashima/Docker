FROM --platform=linux/amd64 ubuntu:latest

RUN apt update -y && apt install -y \
    build-essential \
    bzip2 \
    wget \
    cmake \
    git \
    gcc \
    make && apt clean

ENV USER guest
RUN adduser --system --group $USER
USER $USER
WORKDIR /home/guest


RUN wget -q -O ~/Mambaforge.sh  "https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-$(uname)-$(uname -m).sh" && \
    bash ~/Mambaforge.sh -b -p "/home/guest/conda" && echo ". ~/conda/etc/profile.d/conda.sh" >> ~/.bashrc && rm -rf ~/Mambaforge.sh

RUN git clone https://github.com/Sota-Nakashima/SSERAFIM.git

RUN /home/guest/conda/bin/conda config --append channels bioconda && /home/guest/conda/bin/conda env create --file ~/SSERAFIM/sserafim.yml

ENV PATH $PATH:/home/guest/SSERAFIM

WORKDIR /home/guest/work