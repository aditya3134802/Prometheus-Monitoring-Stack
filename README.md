# Prometheus-Monitoring-Stack
Directory Structure:
prometheus-grafana/
├── docker-compose.yml
└── config/
    ├── prometheus.yml
    └── dashboards/
Key Script:
yaml
# docker-compose.yml
version: '3'
services:
  prometheus:
    image: prom/prometheus
    ports:
      - "9090:9090"
  grafana:
    image: grafana/grafana
    ports:
      - "3000:3000"
      
