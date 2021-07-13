## SAP RFC Overview
![SAP RFC Overview](https://raw.githubusercontent.com/popecruzdt/BizOpsConfiguratorPacks/main/screenshots/Kubernetes_Namespace_Overview.png)

## Summary:
This is a collection of dashboards that present the SAP RFC metrics gathered by the Dynatrace Extension for SAP Application Server.

https://www.dynatrace.com/hub/detail/sap-abap/?query=sap

Developed and tested on Dynatrace v1.221.

## Dashboards:
### SAP RFC - Overview
This dashboard displays the most relevant information about the health, performance, and utilization of each monitored SAP Application Server and the RFC calls.

### SAP RFC - Incoming Performance
This dashboard displays the throughput and response time of incoming RFC calls.  The parent view aggregates all RFC calls.  The incoming performance breakdowns splits the metrics by the selected dimension.

### SAP RFC - Outgoing Performance
This dashboard displays the throughput and response time of outgoing RFC calls.  The parent view aggregates all RFC calls.  The incoming performance breakdowns splits the metrics by the selected dimension.

## Prerequisites:
#### Deploy the SAP Application Server Extension
  * https://www.dynatrace.com/support/help/shortlink/sap-activegate-extension
