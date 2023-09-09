FROM mcr.microsoft.com/devcontainers/python:1-3.10-bullseye

RUN curl https://get.modular.com | \
  MODULAR_AUTH=your_auth_code \
  sh -

RUN modular install mojo

RUN echo 'export MODULAR_HOME="$HOME/.modular"' >> ~/.bashrc

RUN echo 'export PATH="$MODULAR_HOME/pkg/packages.modular.com_mojo/bin:$PATH"' >> ~/.bashrc