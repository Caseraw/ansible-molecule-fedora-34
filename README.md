# Ansible Molecule Fedora 34

[![Docker Repository on Quay](https://quay.io/repository/kasra_amirsarvari/ansible-molecule-fedora-34/status "Docker Repository on Quay")](https://quay.io/repository/kasra_amirsarvari/ansible-molecule-fedora-34) ![GitHub Actions](https://github.com/Caseraw/ansible-molecule-fedora-34/actions/workflows/docker-test-build-push.yml/badge.svg) ![Docker Pulls](https://img.shields.io/docker/pulls/caseraw/ansible-molecule-fedora-34) ![Docker Image Version (tag latest semver)](https://img.shields.io/docker/v/caseraw/ansible-molecule-fedora-34/latest) ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/caseraw/ansible-molecule-fedora-34/latest) ![Docker Stars](https://img.shields.io/docker/stars/caseraw/ansible-molecule-fedora-34)

This container image is made for use with Molecule and Ansible. It contains specific configuration for testing Ansible content. The image is not meant to use for other containerized applications.

The image is based on `quay.io/fedora/fedora` with tag `34-x86_64` at [quay.io](https://quay.io/repository/fedora/fedora?tab=tags) *([upstream fedora](https://registry.fedoraproject.org/repo/fedora/tags/))*

## Get this image

Image is available at **quay.io** and **docker.io**.

```shell
podman pull quay.io/kasra_amirsarvari/ansible-molecule-fedora-34
```
> *https://quay.io/repository/kasra_amirsarvari/ansible-molecule-fedora-34*  

```shell
docker pull docker.io/caseraw/ansible-molecule-fedora-34
```
> *https://hub.docker.com/repository/docker/caseraw/ansible-molecule-fedora-34*  

### Tags

The `latest` tag refers to the latest custom build based on the original base image at `quay.io/fedora/fedora:34-x86_64`.

## Build

```shell
podman build -t quay.io/kasra_amirsarvari/ansible-molecule-fedora-34 .

docker build -t caseraw/ansible-molecule-fedora-34:latest .
```

## Run a container

```shell
docker run -d --name ansible-molecule --privileged=True --volume /sys/fs/cgroup:/sys/fs/cgroup:ro quay.io/kasra_amirsarvari/ansible-molecule-fedora-34:latest /usr/sbin/init

docker run -d --name ansible-molecule --privileged=True --volume /sys/fs/cgroup:/sys/fs/cgroup:ro caseraw/ansible-molecule-fedora-34:latest /usr/sbin/init
```

## CI/CD

The image is built en tested using GitHub Actions, view all the [workflows](https://github.com/Caseraw/ansible-molecule-fedora-34/actions).