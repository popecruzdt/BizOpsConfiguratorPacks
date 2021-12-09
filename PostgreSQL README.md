## PostgreSQL (by popecruzdt)
![Screenshot](https://raw.githubusercontent.com/popecruzdt/BizOpsConfiguratorPacks/main/screenshots/PostgreSQL_Dashboard_screenshot.png)

## Summary:
This is a dashboard that presents the PostgreSQL (postgres) metrics collected by Dynatrace across the various hosting platforms.  Metrics are obtained via OneAgent, Telegraf, and the appropriate cloud provider integration.

https://www.dynatrace.com/hub/?query=postgresql

Developed and tested on Dynatrace v1.231.

## Prerequisites:

### Local (OneAgent) Deployment:
In this scenario, you are hosting the postgres database engine and have access to deploy the Dynatrace OneAgent on the postgres server/host.
#### Deploy the Dynatrace OneAgent on the postgres server/host
  * https://www.dynatrace.com/support/help/shortlink/oneagent-hub
#### Configure the Dynatrace OneAgent PostgreSQL extension for the postgres server/host
  * https://www.dynatrace.com/support/help/shortlink/postgresql-monitoring
#### Deploy Telegraf on the postgres server/host
  * https://docs.influxdata.com/telegraf/v1.20/introduction/installation/
  * https://github.com/influxdata/telegraf/tree/master/plugins/inputs/postgresql
  * https://github.com/influxdata/telegraf/tree/master/plugins/outputs/dynatrace
#### Deploy the Dynatrace OneAgent on the upstream application calling the database
  * https://www.dynatrace.com/support/help/shortlink/oneagent-hub

### AWS RDS (CloudWatch) Deployment:
In this scenario, the postgres database is hosted in AWS, via the Relational Database Server (RDS) cloud native service.
#### Set up AWS monitoring (CloudWatch integration) with ActiveGate (not metric streams)
  * https://www.dynatrace.com/support/help/shortlink/aws-monitor-hub
#### Deploy the Dynatrace OneAgent on the upstream application calling the database
  * https://www.dynatrace.com/support/help/shortlink/oneagent-hub
#### Deploy Telegraf on one (or more) of the upstream application hosts calling the database (if not applicable, install on any host supported by Telegraf)
  * https://docs.influxdata.com/telegraf/v1.20/introduction/installation/
  * https://github.com/influxdata/telegraf/tree/master/plugins/inputs/postgresql
  * https://github.com/influxdata/telegraf/tree/master/plugins/outputs/dynatrace

### AzureDB (Azure Monitor) Deployment:
In this scenario, the postgres database is hosted in Azure, via the Azure Database for PostgreSQL server cloud native service.
#### Set up Azure monitoring (Azure Monitor integration) with ActiveGate
  * https://www.dynatrace.com/support/help/shortlink/azure-monitor-integration
#### Deploy the Dynatrace OneAgent on the upstream application calling the database
  * https://www.dynatrace.com/support/help/shortlink/oneagent-hub
#### Deploy Telegraf on one (or more) of the upstream application hosts calling the database (if not applicable, install on any host supported by Telegraf)
  * https://docs.influxdata.com/telegraf/v1.20/introduction/installation/
  * https://github.com/influxdata/telegraf/tree/master/plugins/inputs/postgresql
  * https://github.com/influxdata/telegraf/tree/master/plugins/outputs/dynatrace

## Issues & Enhancement:
For any issues or requests for enhancement, please open an Issue on the GitHub repo: https://github.com/popecruzdt/BizOpsConfiguratorPacks/issues
