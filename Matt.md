# Notes

### Passwords
* SAP CP Account: OPP362-001 / OPP362-001@teched.cloud.sap / Welcome18 / p2000499901trial / p2000499901
* SCC: Administrator / welcome
* Dynatrace: opp362@cuvox.de / Welcome18
* HANA DB: SYSTEM / A4iProd$teched18
* Managed: matthieu.pelatan@sap.com / Welcome18 / https://tgo909.dynatrace-managed.com/e/2c21afcc-6512-4da3-8b0e-28bad7bbd235/

<br /><br />

### Timing
* Intro: 10 min
* Preparation: 10 min

* Lesson A: 20 min
  * A1: 7 min
  * A2: 6 min
  * A3: 7 min

* Lesson B: 35 min
  * B1: 5 min  
  * B2: 15 min
  * B3: 15 min

* Lesson C: 35 min
  * C1: 5 min
  * C2: 10 min
  * C3: 10 min
  * C4: 10 min

* Wrap-up: 10 min

> Total: 2 hours

<br /><br />

### Scripts

```
script-request-load.exe "https://espmcloudwebp2000499901trial.hanatrial.ondemand.com/espm-cloud-web/espm.svc/Products?$skip=0&$top=20&$orderby=Name%20asc&$inlinecount=allpages" 400
```
<br /><br />

### To dos
- Add link to Philipp tutorial


### To be added somewhere

1. The availability service will not decrease if a product in the cloud is ordered. No logic implemented in the app/backend.

1. No history APIs (only in Cockpit)


Tags
1. Management zones based on Tags
1. Create a dashboard
1. Purepath + backtrace
1. Download oneagent on your machine



[//]: # ( Adding comment
  )

> Note:

https://wiki.scn.sap.com/wiki/display/TechOps/E2E+Trace+involving+SAP+Cloud+Platform
<br>


> Note: https://wiki.scn.sap.com/wiki/display/SMSETUP/End-To-End+HTTP+Trace+Analysis

<br />

Learn how Dynatrace is going to evaluate your environment and raise problems: Thresholds and Baselining https://www.dynatrace.com/support/help/problem-detection-and-analysis/problem-detection/how-are-new-problems-evaluated-and-raised/
Set your SLAs! -> https://www.dynatrace.com/support/help/problem-detection-and-analysis/problem-detection/how-to-adjust-the-sensitivity-of-problem-detection/
Not enough to see the alerts in Dynatrace? Choose what components are specialy important for you with an Alerting Profile and then setup integrations: email, slack, Jira…
https://www.dynatrace.com/support/help/integrations/problem-notification/how-can-i-filter-problem-notifications-with-alerting-profiles/
https://www.dynatrace.com/support/help/integrations/problem-notification/how-do-i-set-up-email-based-problem-notifications/
https://www.dynatrace.com/news/blog/dynatrace-now-speaks-slack/
https://www.dynatrace.com/support/help/integrations/problem-notification/how-do-i-push-problem-notifications-to-jira/

<br />
> Note: https://launchpad.support.sap.com/#/notes/1252944

<br />

> Note add link to Dynatrace documentation + University
https://www.dynatrace.com/support/help/cloud-platforms/cloud-foundry/how-do-i-monitor-sap-cloud-platform/

> Note: change the package.json file --> temp --> Name

> Note: Compatibility matrix: https://www.dynatrace.com/support/help/technology-support/supported-versions-and-environments/technology-support-and-interoperability-matrix/?_ga=2.118404622.667274710.1534773616-1620112228.1509976816
