# hash:sha256:2bb2d430f753f8064bffa62bd7632155de1d120a17354f502093e4021c91bd3d
ARG REGISTRY_HOST
FROM $REGISTRY_HOST/codeocean/py-r:python3.10.12-R4.2.3-IRkernel-ubuntu22.04

ARG DEBIAN_FRONTEND=noninteractive

ARG GIT_ASKPASS
ARG GIT_ACCESS_TOKEN
COPY git-askpass /

RUN mamba install -y \
        anndata==0.9.2 \
        leidenalg==0.10.1 \
        matplotlib==3.7.2 \
        pandas==2.0.3 \
        scanpy==1.9.5 \
    && mamba clean -ya
