## Kubernetes Overview
![Kubernetes Overview](https://raw.githubusercontent.com/popecruzdt/BizOpsConfiguratorPacks/main/screenshots/Kubernetes_Namespace_Overview_screenshot.png)

## Summary:
This repo is a collection of JSON files designed for automating the monitoring of Kubernetes in Dynatrace, with the BizOpsConfigurator.

Developed and tested on Dynatrace v1.229.

## Dashboards:
### Kubernetes Namespace Overview
This dashboard displays the most relevant information about the health, performance, and utilization of deployments within a specific Kubernetes namespace.  Designed for developers and app owners that are new to Dynatrace and need to see how pods, containers, microservices, and supporting infrastructure are performing.

## Prerequisites:
#### Configure at least (1) Management Zone in the Dynatrace environment that includes the following rules
  * Process groups where Kubernetes namespace equals '*your namespace*' and that run on hosts where Kubernetes cluster name equals '*your kubernetes cluster name*'
  * Cloud application namespace where Cloud application namespace name equals '*your namespace*'
  * Kubernetes cluster on hosts where Kubernetes cluster name equals '*your kubernetes cluster name*'

## Issues & Enhancement:
For any issues or requests for enhancement, please open an Issue on the GitHub repo: https://github.com/popecruzdt/BizOpsConfiguratorPacks/issues
