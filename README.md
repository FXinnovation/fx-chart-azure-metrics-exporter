# azure-metrics-exporter
## Description
This chart deploys the azure_metrics_exporter for use with prometheus.

For more information about azure_metrics_exporter: https://github.com/RobustPerception/azure_metrics_exporter

## Values
| Key | Default | Description |
| --- | ------- | ----------- |
| replicaCount | `3` | Number of replicas |
| image.repository | `'fxinnovation/azure_metrics_exporter'` | Repository of the docker image to be used |
| image.tag | `'0.1.0'` | Tag of the docker image to be used |
| image.pullPolicy | `'IfNotPresent'` | Pull policy of the image to be used |
| nameOverride | `''` | overrides the name of the chart |
| fullnameOverride | `''` | overrides the full name of the chart |
| service.type | `'ClusterIP'` | Type of service to be used |
| service.port | `80` | Service port to be used |
| resources.limits.cpu | `100m` | Limit CPU of the container |
| resources.limits.memory | `128Mi` | Memory limit of the container |
| resources.requests.cpu | `10m` | Requested CPU of the container |
| resources.requests.memory | `64Mi` | Memory requested by the container |
| nodeSelector | `{}` | node selection constraint |
| tolerations | `[]` | scheduling tolerations |
| affinity | `{}` | node and inter-pod affinity and ainti-affinity |
| labels | `{}` | labels that will be added on all resources |
| configuration_secret | `` | configuration for azure_metrics_exporter |
