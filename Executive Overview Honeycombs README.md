## Executive Overview (Honeycombs)
Executive Overview (Honeycombs) Dashboard for BizOpsConfigurator

![Executive Overview (Honeycombs)](https://raw.githubusercontent.com/popecruzdt/BizOpsConfiguratorPacks/main/screenshots/Executive_Overview_Honeycombs.png)

## Summary:
This repo is a collection of JSON files designed for automating the deployment of the executive overview (honeycombs) dashboard in Dynatrace, with the BizOpsConfigurator.

Developed and tested on Dynatrace v1.209.  Should be backwards compatible with releases up to 1 year old.

## Dashboards:
### Executive Overview (Honeycombs)
This dashboard utilizes the application, service, database, and host "health" tiles - commonly referred to as honeycombs.  Typically these tiles are added to a dashboard manually whenever a new group of entities is monitored.  With this package for the BizOpsConfigurator, you can automate the dashboard updates while utilizing automatic tagging rules.

## Prerequisites:
#### Tag your monitored entities using automated tags, with key:value pairs
  * Applications -> Tag your Web, Mobile, or Custom applications with a single common tag and different tag values
  * Services -> Tag your Services with a single common tag and different tag values
  * Databases -> Tag your Database Services with a single common tag and different tag values
  * Hosts -> Tag your Hosts with a single common tag and different tag values

Example automated tagging rules:

![Tagging Rules](https://raw.githubusercontent.com/popecruzdt/BizOpsConfiguratorPacks/main/screenshots/Executive_Overview_Honeycombs_Tagging.png)

## Issues & Enhancement:
For any issues or requests for enhancement, please open an Issue on the GitHub repo: https://github.com/popecruzdt/BizOpsConfiguratorPacks/issues
