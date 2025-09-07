# Base image with Python 3.11
FROM mcr.microsoft.com/devcontainers/python:3.11

# Install system libraries required for OpenCV / mediapipe
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
      build-essential \
      libgl1 \
      libglib2.0-0 \
      libsm6 \
      libxrender1 \
      libxext6 \
      ffmpeg \
      git \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace
COPY . /workspace
