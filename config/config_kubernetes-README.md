## Contents:
* managementZone_kubernetes-namespace.json - Template for configuring a Management Zone for each Kubernetes Namespace
* managementZone_kubernetes-cluster.json - Template for configuring a Management Zone for the entire Kubernetes Cluster
* taggingRule_kubernetes-namespace.json - Creates a tagging rule for 1 tag with a value for each Kubernetes Namespace
* taggingRule_kubernetes-pod.json - Creates a tagging rule for 1 tag with a value for each Kubernetes Base Pod

## Variables:
### managementZone_kubernetes-namespace.json:
* managementZone_id -> unique 64 bit identifier of management zone
* managementZone_name -> unique name of management zone
* kubernetes_cluster-name -> name of kubernetes cluster as configured in Dynatrace
* kubernetes_cloud-type -> cloud type for kubernetes cluster nodes (EC2,Azure,Oracle,OpenStack,Google Cloud Platform)
* kubernetes_namespace -> kubernetes namespace for management zone

### managementZone_kubernetes-cluster.json:
* managementZone_id -> unique 64 bit identifier of management zone
* managementZone_name -> unique name of management zone
* kubernetes_cluster-name -> name of kubernetes cluster as configured in Dynatrace
* kubernetes_cloud-type -> cloud type for kubernetes cluster nodes (EC2,Azure,Oracle,OpenStack,Google Cloud Platform)

### taggingRule_kubernetes-namespace.json:
* taggingRule_id -> unique UUID of automatic tag
* taggingRule_name -> unique name of automatic tag
* kubernetes_cluster-name -> name of kubernetes cluster as configured in Dynatrace
* kubernetes_cloud-type -> cloud type for kubernetes cluster nodes (EC2,Azure,Oracle,OpenStack,Google Cloud Platform)

### taggingRule_kubernetes-pod.json:
* taggingRule_id -> unique UUID of automatic tag
* taggingRule_name -> unique name of automatic tag
* kubernetes_cluster-name -> name of kubernetes cluster as configured in Dynatrace
* kubernetes_cloud-type -> cloud type for kubernetes cluster nodes (EC2,Azure,Oracle,OpenStack,Google Cloud Platform)
