# Running Cassandra in Docker

*Notes:* 
- Reference: See [cassandra@dockerhub](https://hub.docker.com/_/cassandra/) for more details.
- Reference:
- See [docker-command-cheat-sheet]() for common usages of docker.
- `ccn` below is short for `cassandra-container-name`.

## Pull Cassandra

`docker pull cassandra:<tag>`
- `docker pull cassandra` to pull the `latest` version.

## Standalone

### starting

`docker run --name <ccn> -d cassandra:<tag>`
### application linking

### cql Linking

`docker run -it --link <ccn>:cassandra --rm cassandra cqlsh cassandra`
- `--rm`: removed automatically when it (cqlsh) exits

OR,

`docker run -it --link <ccn>:cassandra --rm cassandra sh -c 'exec cqlsh "$CASSANDRA_PORT_9042_TCP_ADDR"'`
## Local Cluster

## Multinode Cluster

*Note:* Using the script []() to launch a mutlinode cluster quickly.

### starting some seeds

`docker run --name <ccn> -d -e CASSANDRA_BROADCAST_ADDRESS=<seed-ip> -p 7000:7000 cassandra:<tag>`

### starting others

`docker run --name <ccn> -d -e CASSANDRA_BROADCAST_ADDRESS=<ip> -p 7000:7000 -e CASSANDRA_SEEDS=<seed-ip> cassandra:<tag>`

### verifying cluster

`docker exec -it <ccn> nodetool status`

## Management

### bash

`docker exec -it <ccn> bash`

### logs

`docker logs <ccn>`