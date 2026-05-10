# Grafana Observability Stack

A complete open-source observability stack built using Grafana, Prometheus, Node Exporter, and Docker Compose for real-time infrastructure monitoring.

## Features

* Real-time CPU monitoring
* Memory utilization tracking
* Disk and network metrics
* Prometheus metrics scraping
* Grafana visualization dashboards
* Dockerized setup
* Auto-refreshing live dashboards

## Tech Stack

* Grafana
* Prometheus
* Node Exporter
* Docker
* Docker Compose

## Architecture

Node Exporter → Prometheus → Grafana

## Setup

```bash
docker compose up -d
```

## Services

| Service       | Port |
| ------------- | ---- |
| Grafana       | 3000 |
| Prometheus    | 9090 |
| Node Exporter | 9100 |

## Dashboard

Imported Grafana dashboard:

* Node Exporter Full (ID: 1860)

## Screenshots

(Add screenshots here)

## Future Improvements

* Loki integration
* Alerting setup
* Go application monitoring
* Kubernetes deployment
