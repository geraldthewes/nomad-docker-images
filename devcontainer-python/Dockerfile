# Base devcontainer
FROM mcr.microsoft.com/devcontainers/python:1-3.12-bookworm


# Install qwen code and UV
RUN curl -fsSL https://deb.nodesource.com/setup_24.x | sudo -E bash -
RUN apt-get update && apt-get upgrade -y && apt-get install -y nodejs && apt-get clean && rm -rf /var/lib/apt/lists/* 
RUN npm install -g @qwen-code/qwen-code@latest
RUN curl -LsSf https://astral.sh/uv/install.sh | sh

