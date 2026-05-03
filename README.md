
# Observability Stack — Prometheus + Grafana

Monitoring stack deployed on AWS EC2 with real-time alerting.

## Tools
- **Prometheus** — metrics collection
- **Grafana** — dashboards and visualization  
- **Alertmanager** — alerts to Slack
- **Node Exporter** — host metrics (CPU, memory, disk, network)
- **Flask App** — custom instrumented application

## Architecture
- Instance 1 → Prometheus + Grafana + Alertmanager
- Instance 2 → Node Exporter + Flask App

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
| Alertmanager | http://localhost:9093 |

## Dashboards
- System Metrics — CPU, Memory, Disk, Network
- Flask App — RED Method (Rate, Errors, Duration)
- Prometheus Self Monitoring

## Alerts
- Instance Down → Slack notification
- High CPU > 80%
- High Memory > 85%
- High Disk > 80%
