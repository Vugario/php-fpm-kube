# PHP-FPM Process monitoring through k8s prometheus and grafana
This is a simple example of how to monitor PHP-FPM processes using k8s, prometheus and grafana.

## Setup
- Install [Orbstack](https://orbstack.com) and enable a k8s cluster
- Run `kubectl apply -f kube.yml` to boot everything up
- Visit grafana via `grafana.default.svc.cluster.local:3000`
- Login with `admin` and `admin`
- Add a default source Prometheus through `http://prometheus:9090`
- Import the dashboard from `grafana-dashboard.json`
- Visit the dashboard and see the metrics