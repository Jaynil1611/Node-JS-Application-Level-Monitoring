# Node-JS-Application-Level-Monitoring

![](https://cdn.codersociety.com/uploads/keystone/nodejs-performance-monitoring-with-prometheus-and-grafana.png)

The repository contains a sample Node.js app which integrates the [Prometheus client for node.js](https://github.com/siimon/prom-client) and exposes metrics on [http://localhost:8080/metrics](http://localhost:8080/metrics). The metrics are periodically scraped by [Prometheus](https://prometheus.io) and visualized through a [Grafana](https://grafana.com/oss/grafana) monitoring dashboard.

## Prerequisites

Make sure that you have Docker and Docker Compose installed:

- [Docker Engine](https://docs.docker.com/engine)
- [Docker Compose](https://docs.docker.com/compose)

## Getting started

Clone the repository:

```bash
git clone https://github.com/Jaynil1611/Node-JS-Application-Level-Monitoring
```

Navigate into the project directory:

```bash
cd Node-JS-Application-Level-Monitoring
```

Start the Docker containers:

```bash
docker-compose up -d
```

## Test containers

- Prometheus should be accessible via [http://localhost:9090](http://localhost:9090)
- Grafana should be accessible via [http://localhost:3000](http://localhost:3000)
- Example Node.js server metrics for application monitoring should be accessible via [http://localhost:8080/metrics](http://localhost:8080/metrics)

## Open monitoring dashboards

Open in your web browser the monitoring dashboards:

There are two Application Level Monitoring dashboards for the Node.js app which can be found on

- [Node JS Application Dashboard](http://localhost:3000/d/XzE5uHXMz/node-js-application-complete-dashboard-final?orgId=1&refresh=30s&from=1618494666387&to=1618496466387&var-instance=All&var-interval=1m&var-target=0.05&var-tolerated=0.1&var-restarts_interval=1d)

- [CPU Utilization Dashboard](http://localhost:3000/d/rYdddlPWk/node-exporter-full?orgId=1&refresh=30s)

- [Node JS Application Mini Dashboard](http://localhost:3000/d/PTSqcpJWk/nodejs-application-mini-dashboard?orgId=1&refresh=30s)
