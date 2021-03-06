# Swift for Tensorflow Docker Images

Unofficial Dockerfiles for [Swift for Tensorflow](https://www.tensorflow.org/swift) toolchain.

https://hub.docker.com/r/s4tf/s4tf

Supported tags:
 * [nightly-cpu](nightly/ubuntu/18.04/cpu/Dockerfile)
 * [0.10.0-cpu](0.10/ubuntu/18.04/cpu/Dockerfile)
 * [0.9.0-cpu](0.9/ubuntu/18.04/cpu/Dockerfile)
 * [0.8.0-cpu](0.8/ubuntu/18.04/cpu/Dockerfile)

## Usage Examples

1. Run Swift REPL:
```
docker run --rm -ti --privileged s4tf/s4tf:0.10.0-cpu swift
```

2. Use as base image for something else, 
e.g. See [Dockerfile](https://github.com/vvmnnnkv/s4tf-style-transfer-service/blob/master/Dockerfile) for neural style transfer web service.
