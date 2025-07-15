FROM mcr.microsoft.com/vscode/devcontainers/dotnet:7.0

ARG NODE_VERSION=18
RUN curl -fsSL https://deb.nodesource.com/setup_${NODE_VERSION}.x | bash - \
  && apt-get update \
  && apt-get install -y nodejs docker.io

RUN usermod -aG docker vscode

WORKDIR /workspace
