FROM ubuntu:18.04
LABEL maintainer="Vova Manannikov <vova@promail.spb.ru>"
LABEL Description="Unofficial Swift for TensorFlow Docker Container (CPU)"

RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update && \
    apt-get -q install -y \
    libatomic1 \
    libbsd0 \
    libcurl4 \
    libxml2 \
    tzdata \
    clang \ 
    libpython3-dev \
    libblocksruntime-dev \
    && rm -r /var/lib/apt/lists/*

# Download toolchain, unpack, cleanup and execute permissions for foundation libs
RUN SWIFT_URL=https://storage.googleapis.com/swift-tensorflow-artifacts/releases/v0.6/rc1/swift-tensorflow-RELEASE-0.6-ubuntu18.04.tar.gz \
    && apt-get update \
    && apt-get install -y curl \
    && curl -fSsL $SWIFT_URL -o swift.tar.gz \
    && tar -xzf swift.tar.gz --directory /usr --strip-components=1 \
    && apt-get purge -y curl \
    && apt-get -y autoremove \
    && rm -r /var/lib/apt/lists/* \
    && rm -f swift.tar.gz \
    && chmod -R o+r /usr/lib/swift
