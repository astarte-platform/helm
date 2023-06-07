# astarte-operator

[astarte-operator](https://github.com/astarte-platform/astarte-kubernetes-operator) Astarte Kubernetes Operator.

![Version: 22.11.01](https://img.shields.io/badge/Version-22.11.01-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 22.11.01](https://img.shields.io/badge/AppVersion-22.11.01-informational?style=flat-square)

This chart bootstraps an Astarte Operator deployment on a [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

See the [Astarte Documentation](https://docs.astarte-platform.org/) for more information about the Astarte platform.

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| drf | dario.freddi@ispirata.com |  |

## Source Code

* <https://github.com/astarte-platform/astarte-kubernetes-operator>

## Requirements

Kubernetes: `>= 1.19.0-0`

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"astarte/astarte-kubernetes-operator"` |  |
| image.tag | string | `"22.11.01"` | Overrides the image tag whose default is the chart appVersion. |
| installCRDs | bool | `true` | Whether or not to install Astarte CRDs. |
| replicaCount | int | `1` | The number of Astarte Operator replicas in your cluster. |
| resources | object | `{"limits":{"cpu":"100m","memory":"256Mi"},"requests":{"cpu":"100m","memory":"128Mi"}}` | Resources to assign to each Astarte Operator instance. |

This document was generated from sources using [helm-docs](https://github.com/norwoodj/helm-docs).
