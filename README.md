# Observability Stack — Prometheus + Grafana

A full monitoring stack built on AWS EC2 using Prometheus and Grafana.

## Stack
- Prometheus — metrics collection
- Grafana — visualization
- Node Exporter — host metrics
- Alertmanager — alerting

## Quick Start
```bash
git clone https://github.com/DivyaNitheyan/observability-project.git
cd observability-project
docker compose up -d
```

## Access
| Service | URL |
|---------|-----|
| Prometheus | http://localhost:9090 |
| Grafana | http://localhost:3000 |

## Dashboards
- Prometheus Self Monitoring
- System Metrics — Node Exporter

