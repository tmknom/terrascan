# terrascan

[![CircleCI](https://circleci.com/gh/tmknom/terrascan.svg?style=svg)](https://circleci.com/gh/tmknom/terrascan)
[![Docker Build Status](https://img.shields.io/docker/build/tmknom/terrascan.svg)](https://hub.docker.com/r/tmknom/terrascan/builds/)
[![Docker Automated build](https://img.shields.io/docker/automated/tmknom/terrascan.svg)](https://hub.docker.com/r/tmknom/terrascan/)
[![MicroBadger Size](https://img.shields.io/microbadger/image-size/tmknom/terrascan.svg)](https://microbadger.com/images/tmknom/terrascan)
[![MicroBadger Layers](https://img.shields.io/microbadger/layers/tmknom/terrascan.svg)](https://microbadger.com/images/tmknom/terrascan)
[![License](https://img.shields.io/github/license/tmknom/terrascan.svg)](https://opensource.org/licenses/Apache-2.0)

Dockerfile template.

## Requirements

- [Docker](https://www.docker.com/)

## Usage

```sh
curl -fsSL https://raw.githubusercontent.com/tmknom/terrascan/master/install | sh -s example
cd example
```

## Makefile targets

```text
build                          Build docker image
format                         Format code
help                           Show help
install                        Install requirements
lint                           Lint code
```

## Development

### Installation

```shell
git clone git@github.com:tmknom/terrascan.git
cd terrascan
make install
```

### Deployment

Automatically deployed by "[DockerHub Automated Build](https://docs.docker.com/docker-hub/builds/)" after merge.

### Deployment Pipeline

1. GitHub - Version Control System
   - <https://github.com/tmknom/terrascan>
2. CircleCI - Continuous Integration
   - <https://circleci.com/gh/tmknom/terrascan>
3. Docker Hub - Docker Registry
   - <https://hub.docker.com/r/tmknom/terrascan>
4. MicroBadger - Docker Inspection
   - <https://microbadger.com/images/tmknom/terrascan>

## License

Apache 2 Licensed. See LICENSE for full details.
