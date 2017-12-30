FROM dennis1f/docker-amd64-toolchain:base

LABEL Description="Build environment for monitord" Vendor="Foo" Version="1.0"

RUN apt-get update \
  && apt-get install --no-install-recommends -y \
       libmp3lame-dev \
  && apt-get autoremove -y \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists* \
  && rm -rf /tmp/* /var/tmp/* \
  && rm -rf /usr/share/man/*
