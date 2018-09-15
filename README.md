# lancache-filebeat

Filebeat configuration for lancache servers

## Requirements

- Ubuntu Server 16.04

## Installation

1. `git clone https://github.com/zeropingheroes/lancache-filebeat.git && cd lancache-filebeat`

## Configuration

All configuration is done via environment variables:

1. `cp .env.example .env`
2. `nano .env`

Alternatively you may set each environment variable manually before install by running the following command:

`export VARIABLE=value`

Environment variables:

* `LOGSTASH_HOST` - The host filebeat should connect to and send logs to, e.g. `filebeat.example.com:5044`
* `CACHE_LOGS_DIRECTORY` - The folder containing nginx's logs, which filebeat will ingest, e.g. `/var/lancache/logs`

## Usage

Once the environment variables have been set, run:

`sudo ./install.sh`
