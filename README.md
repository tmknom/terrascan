# terrascan

[![Dockerfile Actions Status](https://github.com/tmknom/terrascan/workflows/Dockerfile/badge.svg)](https://github.com/tmknom/terrascan/actions?query=workflow%3ADockerfile)
[![Shell Script Actions Status](https://github.com/tmknom/terrascan/workflows/Shell%20Script/badge.svg)](https://github.com/tmknom/terrascan/actions?query=workflow%3A%22Shell+Script%22)
[![Markdown Actions Status](https://github.com/tmknom/terrascan/workflows/Markdown/badge.svg)](https://github.com/tmknom/terrascan/actions?query=workflow%3AMarkdown)
[![YAML Actions Status](https://github.com/tmknom/terrascan/workflows/YAML/badge.svg)](https://github.com/tmknom/terrascan/actions?query=workflow%3AYAML)
[![JSON Actions Status](https://github.com/tmknom/terrascan/workflows/JSON/badge.svg)](https://github.com/tmknom/terrascan/actions?query=workflow%3AJSON)

[![Docker Build Status](https://img.shields.io/docker/build/tmknom/terrascan.svg)](https://hub.docker.com/r/tmknom/terrascan/builds/)
[![Docker Automated build](https://img.shields.io/docker/automated/tmknom/terrascan.svg)](https://hub.docker.com/r/tmknom/terrascan/)
[![MicroBadger Size](https://img.shields.io/microbadger/image-size/tmknom/terrascan.svg)](https://microbadger.com/images/tmknom/terrascan)
[![MicroBadger Layers](https://img.shields.io/microbadger/layers/tmknom/terrascan.svg)](https://microbadger.com/images/tmknom/terrascan)
[![License](https://img.shields.io/github/license/tmknom/terrascan.svg)](https://opensource.org/licenses/Apache-2.0)

Collection of security and best practice test for static code analysis of terraform templates.

This is [terrascan](https://github.com/cesar-rodriguez/terrascan) wrapper.

## Requirements

- [Docker](https://www.docker.com/)

## Usage

### Test

```sh
docker run --rm -v "$PWD:/work" tmknom/terrascan --location . --test all
```

### Help

```sh
 docker run --rm tmknom/terrascan
```

## Makefile targets

```text
build                          Build docker image
format                         Format code
help                           Show help
install                        Install requirements
lint                           Lint code
release                        Release
```

## Development

### Installation

```shell
git clone git@github.com:tmknom/terrascan.git
cd terrascan
make install
```

### Deployment

1. Bump [VERSION](https://raw.githubusercontent.com/tmknom/terrascan/master/VERSION) file.
2. Run `make release`.
3. Automatically deployed by "[Docker Hub Automated Build](https://docs.docker.com/docker-hub/builds/)".

### Deployment Pipeline

1. GitHub - Version Control System
   - <https://github.com/tmknom/terrascan>
2. GitHub Actions - Continuous Integration
   - <https://github.com/tmknom/terrascan/actions>
3. Docker Hub - Docker Registry
   - <https://hub.docker.com/r/tmknom/terrascan>
4. MicroBadger - Docker Inspection
   - <https://microbadger.com/images/tmknom/terrascan>

## License

Apache 2 Licensed. See LICENSE for full details.
