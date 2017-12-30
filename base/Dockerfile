FROM ubuntu:17.10

LABEL Description="Foo" Vendor="Foo" Version="1.0"

RUN apt-get update \
  && apt-get install --no-install-recommends -y \
      # toolchain
      build-essential \
      automake \
      autoconf \
      bc \
  && apt-get autoremove -y \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists* \
  && rm -rf /tmp/* /var/tmp/* \
  && rm -rf /usr/share/man/*
