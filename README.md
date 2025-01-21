# Grafana Training

This repository is supposed to run in `GitHub Codespaces`. Start a codespace in your browser here.
You need a private GitHub account to use Codespaces.

## Set-up

By default, the following ports are used

- `Grafana`: 3000 (user: admin, password: training)
- `Prometheus`: 9090
- `Prometheus Windows`: 9091
- `Windows`: 8006

## Docker

Start your Docker containers with `docker compose up`

Stop the Docker containers with `CTRL + C` or `CMD + C`

Start the Windows container and Prometheus Windows with `docker compose -f docker-compose-windows.yml up`

Includes Node-Exporter, Blackbox-Exporter, Filestat-Exporter

## Node Exporter

There is already a `Node exporter` prepared. 
Start it with: `/workspaces/prometheus/node_exporter`

---
## Useful links

- Node Exporter: https://github.com/prometheus/node_exporter
- Windows Exporter: https://github.com/prometheus-community/windows_exporter
- Blackbox Exporter: https://github.com/prometheus/blackbox_exporter
- Filestat Exporter: https://github.com/michael-doubez/filestat_exporter
- Further Prometheus Exporters: https://prometheus.io/docs/instrumenting/exporters/
