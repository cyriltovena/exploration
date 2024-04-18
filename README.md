
# Grafana Exploration

This is a simple example of how to use Explore Metrics, Logs and Traces, all in one place.

## Installation

Make sure you have `docker` and `docker-compose` isntalled on your machine.

First, you need to install the docker plugin for Loki. This plugin will allow you to send logs from your containers to Loki.

```bash
docker plugin install grafana/loki-docker-driver:latest --alias loki --grant-all-permissions
```

This is only required once.

## Running the example

To run the example, you need to run the following command:

```bash
docker-compose up
```

This will start a simple web server that will generate logs and metrics. You can access the web server at `http://localhost:8001/`.
