# contract-dev-docker

Ethereum DApp development environment

## Prerequisite

- Install Docker
- Install docker-compose 

## Run containers

```bash
$ docker-compose -f docker-compose.yml up  # Exit by Ctrl+c

# Running processes in the background
$ docker-compose -f docker-compose.yml up -d 
$ docker-compose -f docker-compose.yml down
```

- truffle
- ganache-cli


## Attach to truffle 

```bash
$ docker exec -it truffle sh
```
