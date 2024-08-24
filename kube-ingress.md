# What is ingress in kunebernetes

In Kubernetes, an Ingress is a resource that manages external access to services within a Kubernetes cluster, typically HTTP and HTTPS traffic. It provides a way to configure and control how requests are routed to your services, offering features such as load balancing, SSL termination, and URL path-based routing.

## Key Components of Ingress

- Ingress Resource

    - Defines how HTTP(S) requests are routed to services based on rules and paths.
    - It specifies how the requests should be handled and forwarded to backend services.

- Ingress Controller

    -  Implements the rules defined in Ingress resources. It is responsible for managing and configuring a load balancer or proxy that routes traffic according to Ingress rules.
    - Examples of Ingress controllers include NGINX Ingress Controller, Traefik, and HAProxy.
