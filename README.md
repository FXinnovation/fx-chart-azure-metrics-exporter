# azure-metrics-exporter
## Description
This chart deploys the azure-metrics-exporter for use with prometheus.

## Values
| Key | Default | Description |
| --- | ------- | ----------- |
| replicaCount | `3` | Number of replicas |
| image.repository | `'fxinnovation/azure_metrics_exporter'` | Repository of the docker image to be used |
| image.tag | `'0.1.0'` | Tag of the docker image to be used |
| image.pullPolicy | `'IfNotPresent'` | Pull policy of the image to be used |
| nameOverride | `''` | |
| fullnameOverride | `''` | |
| service.type | `'ClusterIP'` | Type of service to be used |
| service.port | `80` | Service port to be used |
| resources.limits.cpu | `100m` | |
| resources.limits.memory | `128Mi` | |
| resources.requests.cpu | `10m` | |
| resources.requests.memory | `64Mi` | |
| nodeSelector | `{}` | |
| tolerations | `[]` | |
| affinity | `{}` | |
| labels | `{}` | |
| configuration_secret | `` | |
