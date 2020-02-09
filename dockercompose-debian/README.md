# docker compose with Debian containers

## Introduction

Simple example.
Creates 5 containers:
* 1 priviliged for running ebpflowexport
* 4 unpriviliged for generating/receiving packets (udp iperf client, udp iperf server, tcp iperf client, tcp iperf server)

## Running

```sh
docker-compose up
```

## Testing

Tested on host with Debian sid and Linux kernel:
```
Linux desktop 5.4.0-3-amd64 #1 SMP Debian 5.4.13-1 (2020-01-19) x86_64 GNU/Linux
```
