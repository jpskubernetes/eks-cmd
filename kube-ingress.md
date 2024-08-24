# What is ingress in kunebernetes

In Kubernetes, an Ingress is a resource that manages external access to services within a Kubernetes cluster, typically HTTP and HTTPS traffic.

It provides a way to configure and control how requests are routed to your services, offering features such as load balancing, SSL termination, and URL path-based routing.

## Key Components of Ingress

- Ingress Resource

  - Defines how HTTP(S) requests are routed to services based on rules and paths.
  - It specifies how the requests should be handled and forwarded to backend services.

- Ingress Controller

  - Implements the rules defined in Ingress resources. It is responsible for managing and configuring a load balancer or proxy that routes traffic according to Ingress rules.
  - Examples of Ingress controllers include NGINX Ingress Controller, Traefik, and HAProxy.

### Basic Concepts

- Ingress Rules:

Define how requests should be matched and routed to different services based on the hostnames and paths.
Rules can specify routing to different backend services depending on the request URL.

- Hostnames and Paths:

Ingress rules can match requests based on the host (e.g., example.com) and the URL path (e.g., /api).
This allows you to direct traffic to different services within your cluster.

- TLS Termination:

Ingress can manage SSL/TLS certificates to handle HTTPS traffic. It can terminate SSL connections and forward plain HTTP traffic to backend services.
