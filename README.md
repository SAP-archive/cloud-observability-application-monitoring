# SAP TechEd 2018 
# OPP362 - Debug and Operate Your Cloud Applications Using Monitoring Tools

## Description
This guide has been created for the SAP TechEd 2018 session [OPP362](https://sessioncatalog.sapevents.com/go/agendabuilder.sessions/?l=191&sid=62559_481320&locale=en_US).
Monitoring cloud native applications or solutions running in a hybrid landscape is becoming more and more complex without the right tools. In this session, you will learn how to use the basic monitoring features of the SAP Cloud Platform, how to do end-to-end tracing with the SAP Solution Manager or how to trace each call and spot each bottleneck immediately with Dynatrace.
<br /><br />

## Requirements
- Configuration of on-premise S/4HANA system and activation of Fiori Reference Apps OData Services. See [SAP tutorial](https://www.sap.com/germany/developer/tutorials/cp-connectivity-configure-fiori-reference-apps.html) for more details.
- Installation of Cloud Connector. See [SAP tutorial](https://www.sap.com/germany/developer/tutorials/cp-connectivity-install-cloud-connector.html) for more details.
- Installation of SAP Solution Manager. See [SAP official documentation](https://support.sap.com/en/solution-manager.html) for more details.
- Installation of the NEO Console and configuration of the environment variables to facilitate its usage in the console. See [SAP official documentation](https://help.sap.com/viewer/65de2977205c403bbc107264b8eccf4b/Cloud/en-US/7f4a5cf6-8885-44e4-9efd-6493b62fc1ca.html) for more details.
- Creation of SAP Cloud Platform trial account. See [SAP tutorial](https://www.sap.com/germany/developer/tutorials/hcp-create-trial-account.html) for more details.
- Deployment of the SAP demo app ESPM application. See [Github repository](https://github.com/SAP/cloud-espm-v2) for more details.
- Adaptation of the ESPM application to deploy the retailer app to the Cloud Foundry environment and establish connectivity between Neo and Cloud Foundry environments. See [SAP tutorial](#) for more details.
- Creation of Dynatrace trial environment. See [Dynatrace website](https://www.dynatrace.com/trial/) for more details.
<br /><br />

## Preparation
Before you start the exercises, you need to go through a couple of required preparation steps. See all details [here](/preparation/README.md).
<br /><br />

## Exercises
The actual exercises are grouped into three lessons
* Lesson A: Basic monitoring features of SAP Cloud Platform
  * [Exercise A1 - Availability checks and alerting](/exercises/A1/README.md)
  * [Exercise A2 - Custom metrics](/exercises/A2/README.md)
  * [Exercise A3 - Monitoring API](/exercises/A3/README.md)
* Lesson B: Trace analysis using SAP Solution Manager
  * [Exercise B1 - Getting started](/exercises/B1/README.md)
  * [Exercise B2 - Configuration](/exercises/B2/README.md)
  * [Exercise B3 - End-to-end tracing](/exercises/B3/README.md)
* Lesson C: Application performance using Dynatrace
  * [Exercise C1 - Getting started](/exercises/C1/README.md)
  * [Exercise C2 - Configuration](/exercises/C2/README.md)
  * [Exercise C3 - Alerting](/exercises/C3/README.md)
  * [Exercise C4 - Root-cause analysis](/exercises/C4/README.md)
<br /><br />

## Handy links
* [SAP Cloud Platform Trial](https://account.hanatrial.ondemand.com/cockpit#/home/trialhome)
* [Cloud Connector](https://localhost:8443)
* SAP official documentation:
  * [Neo console client commands](https://help.sap.com/viewer/65de2977205c403bbc107264b8eccf4b/Cloud/en-US/56e309f496cc446ba441d862db94cb18.html)
  * [Configuring and Executing End-to-End Trace Analysis](https://help.sap.com/viewer/65de2977205c403bbc107264b8eccf4b/Cloud/en-US/a1e3101e108a4ca7a2a8c62654534ef8.html)
  * [Agent Activation for dynatrace](https://help.sap.com/viewer/1078be95fa054ae4ba3021a670248da9/Cloud/en-US/157d85927bc84ae88e314f36ef2a89cc.html)
* [Dynatrace environment](https://tgo909.dynatrace-managed.com)
* [Dynatrace documentation](https://www.dynatrace.com/support/doc/)
<br /><br />

## How to obtain support
If you need any support, have any question, or have found a bug, please report it as an issue in the repository.
<br /><br />

## Known Issues
Currently there are no known issues.
<br /><br />

## Contact
This content is currently maintained by [Matthieu Pelatan](mailto:matthieu.pelatan@sap.com).
<br /><br />

## License
Copyright (c) 2018 SAP SE or an SAP affiliate company. All rights reserved.

This project is licensed under the Apache Software License, v. 2 except as noted otherwise in the  [LICENSE](LICENSE.txt) file.
