## Kubernetes Overview
![Kubernetes Overview](https://raw.githubusercontent.com/popecruzdt/BizOpsConfiguratorPacks/main/screenshots/Kubernetes_Namespace_Overview.png)

## Summary:
This repo is a collection of JSON files designed for automating the monitoring of Kubernetes in Dynatrace, with the BizOpsConfigurator.

Developed and tested on Dynatrace v1.196.

## Dashboards:
### Kubernetes Namespace Overview
This dashboard displays the most relevant information about the health, performance, and utilization of deployments within a specific Kubernetes namespace.  Designed for developers and app owners that are new to Dynatrace and need to see how pods, containers, microservices, and supporting infrastructure are performing.

## Prerequisites:
#### Identify your Kubernetes cloud type and (3) character abbreviation
  * Kubernetes -> k8s (vanilla Kubernetes where you don't care to specify the cloud type)
  * OpenShift -> ocp (OpenShift Container Platform https://www.openshift.com/products/container-platform)
  * Elastic Kubernetes Service -> eks (AWS Kubernetes https://aws.amazon.com/eks/)
  * Azure Kubernetes Service -> aks (Azure Kubernetes https://docs.microsoft.com/en-us/azure/aks/)
  * Google Kubernetes Engine -> gke (Google Kubernetes https://cloud.google.com/kubernetes-engine)
#### Configure at least (1) Management Zone in the Dynatrace environment that includes the following rules
  * Process groups where Kubernetes namespace equals '*your namespace*' and that run on hosts where Kubernetes cluster name equals '*your kubernetes cluster name*'
  * Cloud application namespace where Cloud application namespace name equals '*your namespace*'
  * Kubernetes cluster on hosts where Kubernetes cluster name equals '*your kubernetes cluster name*'
