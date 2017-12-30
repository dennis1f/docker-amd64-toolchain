FROM dennis1f/docker-amd64-toolchain:base

LABEL Description="Build environment for monitord (full)" Vendor="Foo" Version="1.0"

RUN apt-get update \
  && apt-get install --no-install-recommends -y \
       libmariadbclient-dev \
       libpulse-dev \
       libmp3lame-dev \
  && apt-get autoremove -y \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists* \
  && rm -rf /tmp/* /var/tmp/* \
  && rm -rf /usr/share/man/*
