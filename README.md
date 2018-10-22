### Description
This repository contains a step-by-step-guide for configuring and running a Mixed-mode (Hybrid) Cloud Foundry application that interacts with an on-premises Gateway system. This guide has been adapted from the TechEd 2017 session [CPL360](https://sessioncatalog.sapevents.com/go/agendabuilder.sessions/?l=157&sid=49863_470530&locale=en_US). This material has been prepared for the Spring 2018 Presales Learn to Win Week hands-on training.

### Requirements
Basically, you just need your SAP laptop to complete these exercises.

### Exercises

The actual exercises are grouped into three lessons
* Lesson A
  * [Exercise A1](/exercises/A1/README.md)
  * [Exercise A2](/exercises/A2/README.md)
  * [Exercise A3](/exercises/A3/README.md)
* Lesson B
  * [Exercise B1](/exercises/B1/README.md)
  * [Exercise B2](/exercises/B2/README.md)
  * [Exercise B3](/exercises/B3/README.md)
* Lesson C
  * [Exercise C1](/exercises/C1/README.md)
  * [Exercise C2](/exercises/C2/README.md)

### Handy links
Most of the screenshots in this lab material were taken using SAP's internal Canary Cloud Foundry.  You can perform this lab with Public Trial accounts too, but some of the URLs and hosts will differ.

Here are some handy URLS that will be unique to each environment; you can copy and paste them as needed:

|CF Environment|URLs / Hosts                                                        |
|--------------|--------------------------------------------------------------------|
| Canary CF    | Login URL: https://account.int.sap.hana.ondemand.com/cockpit <br /> SCC Landscape Host: **`cf.sap.hana.ondemand.com`** <br />cf API URL: https://api.cf.sap.hana.ondemand.com |
| CF Trial EU/AWS    | Login URL: https://account.hanatrial.ondemand.com/cockpit <br />SCC Landscape Host: **`cf.eu10.hana.ondemand.com`** <br />cf API URL: https://api.cf.eu10.hana.ondemand.com |
| CF Trial US/AWS    | Login URL: https://account.hanatrial.ondemand.com/cockpit <br />SCC Landscape Host: **`cf.us10.hana.ondemand.com`** <br />cf API URL: https://api.cf.us10.hana.ondemand.com |

### How to obtain support
If you need any support, have any question, or have found a bug, please report it as an issue in the repository.

The unmodified version of the Node.js main app sample use in this lab can be found on SAP's internal Github: https://github.wdf.sap.corp/Connectivity-CF-PM/cloud-platform-cf-connectivity-principal-propagation


### Known Issues
Currently there are no known issues.

### Contacts
This lab content is currently maintained by [Philipp Stehle](mailto:philipp.stehle@sap.com) and [Matthieu Pelatan](mailto:matthieu.pelatan@sap.com).

### License
Copyright (c) 2018 SAP SE or an SAP affiliate company. All rights reserved.
This file is licensed under the Apache Software License, v. 2 except as noted otherwise in the  [LICENSE](LICENSE) file.
