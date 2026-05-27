FROM nvidia/cuda:12.6.0-cudnn-devel-ubuntu22.04

ENV DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Shanghai

# =========================
# System Dependencies
# =========================
RUN apt-get update && apt-get install -y \
    python3.10 \
    python3-pip \
    python3-dev \
    python3-venv \
    build-essential \
    git \
    curl \
    wget \
    unzip \
    vim \
    tmux \
    htop \
    ffmpeg \
    libgl1 \
    libglib2.0-0 \
    libsm6 \
    libxext6 \
    libxrender-dev \
    libglfw3 \
    libglew-dev \
    libosmesa6-dev \
    xvfb \
    && rm -rf /var/lib/apt/lists/*

# =========================
# Python
# =========================
RUN python3 -m pip install --upgrade pip setuptools wheel

# =========================
# PyTorch (CUDA 12.6)
# =========================
RUN pip install \
    torch \
    torchvision \
    torchaudio

# =========================
# Workspace
# =========================
WORKDIR /workspace

CMD ["/bin/bash"]