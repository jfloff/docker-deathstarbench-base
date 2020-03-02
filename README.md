# DeathStarBench Base

[![Docker Stars](https://img.shields.io/docker/stars/jfloff/deathstarbench-base.svg)][hub]
[![Docker Pulls](https://img.shields.io/docker/pulls/jfloff/deathstarbench-base.svg)][hub]
[![Build Status](https://travis-ci.org/jfloff/docker-deathstarbench-base.svg?branch=master)][travis]

[hub]: https://hub.docker.com/r/jfloff/docker-deathstarbench-base
[travis]: https://travis-ci.org/jfloff/docker-deathstarbench-base

Docker image for [DeathStarBench](https://github.com/delimitrou/DeathStarBench) microservices build.

<!-- MDTOC maxdepth:6 firsth1:0 numbering:0 flatten:0 bullets:1 updateOnSave:1 -->

- [DeathStarBench Base](#deathstarbench-base)
  - [Supported tags](#supported-tags)
  - [Details](#details)
  - [Usage](#usage)
  - [License](#license)

<!-- /MDTOC -->

## Supported tags
* **`cpp` ([cpp/Dockerfile](https://github.com/jfloff/docker-deathstarbench-base/blob/master/cpp/Dockerfile))**

## Details
* Installs `mongo-c-driver` for services that connect with a MongoDB database
* Installs `lib-thrift` for services that use Apache Thrift to communicate
* Installs `nlohmann/json` package for [modern JSON](https://github.com/nlohmann/json).
* Installs `yaml-cpp` for YAML files
* Installs `cpp_redis` for communicating with Redis instances
* Installs `opentracing-cpp`, `jaeger-client-cpp`, `protobuf`, `xtrace` for using XTrace and baggages context

## Usage

This image is better used as a base for each microservice in the DeathStarBench benchamark.
```shell
FROM jfloff/deathstarbench-base:cpp
```

## License
The code in this repository follows the same licensing as the original [DeathStarBench](https://github.com/delimitrou/DeathStarBench).
