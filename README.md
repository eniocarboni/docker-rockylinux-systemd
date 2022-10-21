# Rocky Linux 8 Docker Image with systemd

[![Build](https://github.com/eniocarboni/docker-rockylinux-systemd/actions/workflows/build.yml/badge.svg?branch=8)](https://github.com/eniocarboni/docker-rockylinux-systemd/actions/workflows/build.yml) [![GPL License](https://img.shields.io/badge/license-GPL-blue.svg)](https://www.gnu.org/licenses/) [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/EnioCarboni)

Rocky Linux 8 Docker container with systemd, useful for tests with `ansible` especially with `molecule`

## Tags

  - `8` on [8 branch](https://github.com/eniocarboni/docker-rockylinux-systemd/tree/8)


## How to Build

  * Verify if [Docker is installed](https://docs.docker.com/install/).
  * Run on main branch: `docker build -t docker-rockylinux-systemd:8 .`
  * Verify image: `docker images`

## How to Use

  * `docker pull eniocarboni/docker-rockylinux-systemd:8` (or use the image you built earlier).
  * `docker run --detach --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro eniocarboni/docker-rockylinux-systemd:8`

View the run container with

  * `docker ps`

Enter in the container with:

  * `docker exec -it <container_id> bash`

Kill container with:

  * `docker kill <container_id>`

Remove container with:

  * `docker image rm -f <container_id>` 

## Author

Created in 2022 by Enio Carboni

## License

GNU GENERAL PUBLIC LICENSE (see [LICENSE](LICENSE) file)
