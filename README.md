# Grafana Training

This repository is supposed to run in `GitHub Codespaces`. Start a codespace in your browser here.
You need a private GitHub account to use Codespaces.

## Set-up

By default, the following ports are used

- `Grafana`: 3000 (user: admin, password: training)
- `Prometheus`: 9090
- `Windows`: 8006

Every exercise directory contains a `/init` and a `/solution` directory to start your exercise.

Use the `/init` directory to start with the prepared exercise.
The `/solution` directory contains an example solution for the current exercise.

### Docker

Start your Docker containers in the particular directory with `docker compose up`

Stop the Docker containers with `CTRL + C` or `CMD + C`

---
## Exercises

### Exercise 1 - Node Exporter

Enter the exercise with `cd $WD/exercise-1/init`

There is already a `Node exporter` prepared.
Start it with: `/workspaces/prometheus/node_exporter`

## Exercise 2 - Filestat Exporter

Enter the exercise with `cd $WD/exercise-2/init`

Monitor all files within the `/filestat` directory via Filestat Exporter.

## Exercise 3 - Blackbox Exporter

Enter the exercise with `cd $WD/exercise-3/init`

Monitor the url http://prometheus.io via Blackbox Exporter.

## Exercise 4 - Windows Exporter

Enter the exercise with `cd $WD/exercise-4`

This exercise is already set up to view the Windows Exporter.
At the first start-up with `docker compose up` the installation of Windows inside a Docker container
will take several minutes!

After the first installation IIS will be activated and a Windows Exporter will be started.

You can access the Windows machine at port 8006.

Check the Grafana dashboard _Windows Exporter Dashboard_.

---
## Useful links

- Node Exporter: https://github.com/prometheus/node_exporter
- Windows Exporter: https://github.com/prometheus-community/windows_exporter
- Blackbox Exporter: https://github.com/prometheus/blackbox_exporter
- Filestat Exporter: https://github.com/michael-doubez/filestat_exporter
- Further Prometheus Exporters: https://prometheus.io/docs/instrumenting/exporters/
