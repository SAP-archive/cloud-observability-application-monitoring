# Lesson C: Application performance using Dynatrace
# Exercise C3: Alerting

#### Objective
In this exercise, you will learn how to define the preferred method to receive real-time notifications related to problems in your environment. Then you will configure detection sensitivity and set alert thresholds for infrastructure components or certain services.<br /><br />

#### Estimated time
10 minutes
<br />
<br />

## 1. Notification configuration
1. First we need to configure the way alerts will be sent. From the dashboard, click on the tile called **Problem**.<br /><br />
  ![](../../images/c3-dt-dashboard.png)<br /><br />

1. Click on **Set up notifications** to jump directly to the right settings section.<br /><br />
  ![](../../images/c3-dt-alert-01.png)<br /><br />

1. Press the button **Set up notifications**.<br /><br />
  ![](../../images/c3-dt-alert-02.png)<br /><br />

1. Click on **Email** to get the alert sent to your email address.<br /><br />
    ![](../../images/c3-dt-alert-03.png)<br /><br />

1. Add a meaninful display name and an email address to get the notifications. If you don't want to put your own email address, you can use a service like [Mailinator](https://www.mailinator.com).<br /><br />
    ![](../../images/c3-dt-alert-04.png)<br /><br />

1. Then scroll down and send a test notification before saving the configuration.<br /><br />
    ![](../../images/c3-dt-alert-05.png)<br /><br />

## 2. Infrastructure alerts
1. Let us now refine the default configuration of the Dynatrace alerts for infrastructure. Expend the section **Anomaly detection** and click **Infrastrucure**.<br /><br />
    ![](../../images/c3-dt-alert-infra-01.png)<br /><br />

1. Go to **Detect CPU saturation host** and select **based on custom settings** in the dropdown list.<br /><br />
    ![](../../images/c3-dt-alert-infra-02.png)<br /><br />

1. Change the standard threshold from 95% to 80%.<br /><br />
    ![](../../images/c3-dt-alert-infra-03.png)<br /><br />

## 3. Services alerts
1. Dynatrace compares out-of-the box the current behavior of services to a reference period up to 7 days and send alerts if something differs from the baseline. As we don't have such data now, let us configure the detection sensitivity and the alert thresholds. Under **Anomaly detection** click **Services**.<br /><br />
    ![](../../images/c3-dt-alert-services-01.png)<br /><br />

1. Go to **Detect response time degradations** and select **using fixed thresholds** in the dropdown list.<br /><br />
    ![](../../images/c3-dt-alert-services-02.png)<br /><br />

1. Add the failure --> using fixed + 0%

1. In the over-alerting settings, change the value from **10** to **1** and set the sensitivity to **High**.<br /><br />
   ![](../../images/c3-dt-alert-services-03.png)<br /><br />

1. Go to **Detect increases in failure rate** and select **using fixed thresholds** in the dropdown list.<br /><br />
  ![](../../images/c3-dt-alert-services-04.png)

<br /><br /><br />


![](../../images/nav.png) [Previous exercise](../C2/README.md) ｜ [Next exercise](../C4/README.md) ｜ [Overview page](../../README.md)
