# prometheus-mailgun-exporter

Prometheus Mailgun Exporter

## Build

`make` will build both binary and Docker image

## Run

The exporter will serve metrics on `http://<ip>:9616/metrics`

`export MG_API_KEY=<api_key>`
`export MG_DOMAIN=<domain>`

- Docker
  1. `docker run -ti --rm --name prometheus-mailgun-exporter -e MG_API_KEY=<key> -e MG_DOMAIN=<domain> casestack/prometheus-mailgun-exporter:latest`
- Binary
  1. `./prometheus-mailgun-exporter`

## Europe Users

`export API_BASE=https://api.eu.mailgun.net/v3`

## Dashboard

The Grafana dashboard can be found [here](https://grafana.com/grafana/dashboards/10663)
