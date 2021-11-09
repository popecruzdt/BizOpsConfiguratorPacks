## Kubernetes Namespace Overview
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
  * Services on Process groups where Kubernetes namespace equals '*your namespace*'
  * Kubernetes namespace where Kubernetes namespace name equals '*your namespace*'
  * Kubernetes workloads on Kubernetes namespace where Kubernetes namespace name equals '*your namespace*'
  * Cloud application namespace where Cloud application namespace name equals '*your namespace*'
  * Kubernetes cluster on hosts where Kubernetes cluster name equals '*your kubernetes cluster name*'

![Management Zone](https://raw.githubusercontent.com/popecruzdt/BizOpsConfiguratorPacks/main/screenshots/Kubernetes_Namespace_Overview_management_zone_screenshot.png)
#### (Optional) Configure (2) log metrics to track Kubernetes Events for your namespaces.
  * INFO Events by namespace and reason
  * WARN Events by namespace and reason

![INFO Events](https://raw.githubusercontent.com/popecruzdt/BizOpsConfiguratorPacks/main/screenshots/Kubernetes_Namespace_Overview_events_metric_info_screenshot.png)
![WARN Events](https://raw.githubusercontent.com/popecruzdt/BizOpsConfiguratorPacks/main/screenshots/Kubernetes_Namespace_Overview_events_metric_warn_screenshot.png)

Note, this requires Log Monitoring v2.

## Issues & Enhancement:
For any issues or requests for enhancement, please open an Issue on the GitHub repo: https://github.com/popecruzdt/BizOpsConfiguratorPacks/issues
