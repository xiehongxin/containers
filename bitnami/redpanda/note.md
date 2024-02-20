# Redpanda Note

## doc
https://github.com/redpanda-data/redpanda

## install
curl -1sLf \
'https://dl.redpanda.com/nzc4ZYQK3WRGd9sy/redpanda/cfg/setup/bash.deb.sh' \
| sudo -E bash

sudo apt-get install redpanda
sudo apt-get install redpanda-console

## service
/lib/systemd/system/redpanda.service
/lib/systemd/system/redpanda-console.service

## config
/etc/redpanda/redpanda.yaml
/etc/redpanda/redpanda-console-config.yaml

## dashboard
env KAFKA_BROKERS=0.0.0.0:9092 SERVER_LISTENPORT=8083 redpanda-console  (visit localhost:8083)