# contract-dev-docker

Ethereum DApp development environment

## Prerequisite

- Install Docker
- Install docker-compose 

## Run containers


```bash
$ docker-compose -f docker-compose.yml up  # Exit by Ctrl+C
```

```
# Running processes in the background
$ docker-compose -f docker-compose.yml up -d 
$ docker-compose -f docker-compose.yml down
```

- truffle
- ganache-cli


## Attach to truffle and see wehther the env works 

```bash
$ docker exec -it truffle sh
$ cd hello/
$ truffle migrate --network dev
```
