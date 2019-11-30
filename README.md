# Swift for Tensorflow Dockerfiles

Unofficial Dockerfiles for [Swift for Tensorflow](https://www.tensorflow.org/swift) toolchain.

https://hub.docker.com/r/s4tf/s4tf

Supported tags:
 * [nightly-cpu](nightly/ubuntu/18.04/cpu/Dockerfile)
 * [0.6.0-cpu](0.6/ubuntu/18.04/cpu/Dockerfile)
 * [0.5.0-cpu](0.5/ubuntu/18.04/cpu/Dockerfile)
 * [0.4.0-cpu](0.4/ubuntu/18.04/cpu/Dockerfile)

## Usage Examples

1. Run Swift REPL:
```
docker run --rm -ti --privileged s4tf/s4tf:0.6.0-cpu swift
```

2. Use as base image for something else, 
e.g. See [Dockerfile](https://github.com/vvmnnnkv/s4tf-style-transfer-service/blob/master/Dockerfile) for neural style transfer web service.
