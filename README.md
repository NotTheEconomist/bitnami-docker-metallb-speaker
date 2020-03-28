
# What is MetalLB Speaker?

> MetalLB is a load-balancer that allows enabling "LoadBalancer" service addresses in any bare-metal Kubernetes installation. MetalLB speaker is the per-node daemon that advertises services with assigned IPs.

[Overview of metallb](https://metallb.universe.tf/)

# TL;DR;

```bash
$ docker run --name metallb-speaker bitnami/metallb-speaker:latest
```

# Why use Bitnami Images?

* Bitnami closely tracks upstream source changes and promptly publishes new versions of this image using our automated systems.
* With Bitnami images the latest bug fixes and features are available as soon as possible.
* Bitnami containers, virtual machines and cloud images use the same components and configuration approach - making it easy to switch between formats based on your project needs.
* All our images are based on [minideb](https://github.com/bitnami/minideb) a minimalist Debian based container image which gives you a small base container image and the familiarity of a leading linux distribution.
* All Bitnami images available in Docker Hub are signed with [Docker Content Trust (DTC)](https://docs.docker.com/engine/security/trust/content_trust/). You can use `DOCKER_CONTENT_TRUST=1` to verify the integrity of the images.
* Bitnami container images are released daily with the latest distribution packages available.


> This [CVE scan report](https://quay.io/repository/bitnami/metallb-speaker?tab=tags) contains a security report with all open CVEs. To get the list of actionable security issues, find the "latest" tag, click the vulnerability report link under the corresponding "Security scan" field and then select the "Only show fixable" filter on the next page.

# Supported tags and respective `Dockerfile` links

> NOTE: Debian 9 and Oracle Linux 7 images have been deprecated in favor of Debian 10 images. Bitnami will not longer publish new Docker images based on Debian 9 or Oracle Linux 7.

Learn more about the Bitnami tagging policy and the difference between rolling tags and immutable tags [in our documentation page](https://docs.bitnami.com/containers/how-to/understand-rolling-tags-containers/).


* [`0-debian-10`, `0.9.3-debian-10-r1`, `0`, `0.9.3`, `latest` (0/debian-10/Dockerfile)](https://github.com/bitnami/bitnami-docker-metallb-speaker/blob/0.9.3-debian-10-r1/0/debian-10/Dockerfile)

Subscribe to project updates by watching the [bitnami/metallb-speaker GitHub repo](https://github.com/bitnami/bitnami-docker-metallb-speaker).

# Get this image

The recommended way to get the Bitnami metallb-speaker Docker Image is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/r/bitnami/metallb-speaker).

```bash
$ docker pull bitnami/metallb-speaker:latest
```

To use a specific version, you can pull a versioned tag. You can view the [list of available versions](https://hub.docker.com/r/bitnami/metallb-speaker/tags/) in the Docker Hub Registry.

```bash
$ docker pull bitnami/metallb-speaker:[TAG]
```

If you wish, you can also build the image yourself.

```bash
$ docker build -t bitnami/metallb-speaker:latest 'https://github.com/bitnami/bitnami-docker-metallb-speaker.git#master:0/debian-10'
```

# Configuration

## Running commands

To run commands inside this container you can use `docker run`, for example to execute `metallb-speaker --version` you can follow the example below:

```bash
$ docker run --rm --name metallb-speaker bitnami/metallb-speaker:latest -- --version
```

Consult the [metallb Reference Documentation](https://metallb.universe.tf/configuration/) to find the available configuration parameters. Note that this container is expected to be used in a Kubernetes cluster.

# Contributing

We'd love for you to contribute to this container. You can request new features by creating an [issue](https://github.com/bitnami/bitnami-docker-metallb-speaker/issues), or submit a [pull request](https://github.com/bitnami/bitnami-docker-metallb-speaker/pulls) with your contribution.

# Issues

If you encountered a problem running this container, you can file an [issue](https://github.com/bitnami/bitnami-docker-metallb-speaker/issues/new). For us to provide better support, be sure to include the following information in your issue:

- Host OS and version
- Docker version (`docker version`)
- Output of `docker info`
- Version of this container
- The command you used to run the container, and any relevant output you saw (masking any sensitive information)

# License

Copyright 2020 Bitnami

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.