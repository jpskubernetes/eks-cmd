# HEALTH CHECK - Liveness and Readiness Probes in Kubernetes

components of Kubernetes deployments for ensuring application health and availability.

## Liveness Probes

- `Purpose`: Determine if an application is alive and functioning correctly.
- `Action`: If a liveness probe fails, Kubernetes restarts the pod.
Types:
- `HTTP Get`: Sends an HTTP GET request to a specified path.
- `TCP Socket`: Attempts to connect to a specified port.
- `Exec`: Executes a command within the container.

## Readiness Probes

- `Purpose`: Determine if an application is ready to receive traffic.
- `Action`: If a readiness probe fails, Kubernetes removes the pod from service discovery.
Types:
- `HTTP Get`: Sends an HTTP GET request to a specified path.
- `TCP Socket`: Attempts to connect to a specified port.
- `Exec`: Executes a command within the container.
