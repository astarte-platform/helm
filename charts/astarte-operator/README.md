# astarte-operator

[astarte-operator](https://github.com/astarte-platform/astarte-kubernetes-operator) Astarte Kubernetes Operator.

![Version: 26.7.0-rc.0](https://img.shields.io/badge/Version-26.7.0--rc.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 26.7.0-rc.0](https://img.shields.io/badge/AppVersion-26.7.0--rc.0-informational?style=flat-square)

This chart bootstraps an Astarte Operator deployment on a [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

See the [Astarte Documentation](https://docs.astarte-platform.org/) for more information about the Astarte platform.

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| matt-mazzucato | mattia.mazzucato@secomind.com |  |
| annopaolo | arnaldo.cesco@secomind.com |  |
| lucamarchiori | luca.marchiori@secomind.com |  |
| guicrocetti | guilherme.crocetti@secomind.com |  |

## Source Code

* <https://github.com/astarte-platform/astarte-kubernetes-operator>

## Requirements

Kubernetes: `>= 1.19.0-0`

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"astarte/astarte-kubernetes-operator"` |  |
| image.tag | string | `"26.7.0-rc.0"` | Overrides the image tag whose default is the chart appVersion. |
| installCRDs | bool | `true` | Whether or not to install Astarte CRDs. |
| metrics | object | `{"enable":false,"port":8443,"secure":true}` | Metrics configuration. Metrics are exposed on the configured port. When enabled, they use HTTPS by default. |
| metrics.enable | bool | `false` | Whether to enable the metrics endpoint. |
| metrics.port | int | `8443` | The port to expose metrics on. |
| metrics.secure | bool | `true` | Whether to serve metrics over HTTPS. Set to false to use HTTP. |
| replicaCount | int | `1` | The number of Astarte Operator replicas in your cluster. |
| resources | object | `{"limits":{"cpu":"100m","memory":"256Mi"},"requests":{"cpu":"100m","memory":"128Mi"}}` | Resources to assign to each Astarte Operator instance. |

This document was generated from sources using [helm-docs](https://github.com/norwoodj/helm-docs).
