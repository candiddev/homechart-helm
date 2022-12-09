# Homechart Helm Chart

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/homechart)](https://artifacthub.io/packages/search?repo=homechart)

> Run [Homechart](https://homechart.app) on Kubernetes via Helm.

Checkout our [docs](https://docs.homechart.app) for more details on self hosting Homechart!

## Getting Started

Using the Helm Chart is easy:

```
helm repo add homechart https://helm.homechart.app/
helm install my-homechart homechart/homechart
```

## Defaults

The Homechart Helm Chart creates a Homechart Deployment and a PostgreSQL StatefulSet and sets the appropriate values for these to work out of the box.  Users can bring their own PostgreSQL instance by setting `postgresql.enabled` to false and setting the appropriate config values in homechart.config.secrets and homechart.config.values.  See our [configuration documentation](https://docs.homechart.app/getting-started/on-your-network/installation/configuration-options/) for a full list of supported configuration options.
