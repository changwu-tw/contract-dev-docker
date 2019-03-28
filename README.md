# contract-dev-docker

Ethereum DApp development environment

The training environment is set up by using Docker Compose. The setup consists of two containers that run different services.

- truffle
- ganache-cli

## Requirements

1. You need to have `Docker` and `docker-compose` installed on your machine. Docker is available for MacOS, Linux, and Windows.
2. Install [git](https://git-scm.com/downloads)

### MacOS

- Install [Docker Desktop for Mac](https://docs.docker.com/docker-for-mac/install/)

### Linux

```
# Install docker
$ curl -fsSL https://get.docker.com -o get-docker.sh
$ sh get-docker.sh

# Open a new terminal

# Install docker-compose
$ sudo curl -L https://github.com/docker/compose/releases/download/1.23.2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
```

### Windows

- Install [Docker Desktop for Windows](https://docs.docker.com/docker-for-windows/install/)


### Verify Installation Success

```
$ docker -v
Docker version 18.09.2, build 6247962
$ docker-compose -v
docker-compose version 1.23.2, build 1110ad01
```

## Get docker compose configuration

Clone the git repository for the training environment

```
$ git clone https://github.com/changwu-tw/contract-dev-docker.git
```

### Run containers

Open a terminal

```bash
$ docker-compose -f docker-compose.yml up

# Exit by Ctrl+C
```

Or run the process in the background

```
$ docker-compose -f docker-compose.yml up -d
$ docker-compose -f docker-compose.yml down
```

### Attach to truffle and see wehther the env works

```bash
$ docker exec -it truffle sh
$ cd hello/
$ truffle migrate --network dev
```
