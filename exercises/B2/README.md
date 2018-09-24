# Lesson B: Trace analysis using SAP Solution Manager
# Exercise B2: Configuration

#### Objective
In this exercise, you will learn how to configure the connection to your ABAP system and your SAP cloud Platform subaccount for retrieving the statistical data and enabling the end-to-end trace analysis.<br /><br />

#### Estimated time
15 minutes
<br />
<br />

## 1. Technical systems configuration
1. Double-click the favorite **SAP Solution Manager Configuratons** (Transation SOLMAN_SETUP).<br /><br />
![](../../images/b2-te2-solman_setup.png)<br /><br />
<br /><br />

1. A new window in your browser will open automatically. Close the first popup by clicking on the button **Continue**.<br /><br />
![](../../images/b2-te2-solman_setup-popup.png)<br /><br />
<br /><br />

1. Click on **Managed Systems Configuration** in the left menu. Then choose the ABAP backend system **TE3** and under **Configure System** click **Full Configuration**.
<br /><br />
![](../../images/b2-te2-managed-systems.png)<br /><br />
<br /><br />

1. In the first step called **Assign Product**, press first the **Edit** button and click **Set Automatically**.<br /><br />
![](../../images/b2-te2-assign-product.png)<br /><br />
<br /><br />

1. Click now on the third step called **Maintain RFCs** and select the client **001**.<br /><br />
![](../../images/b2-te2-maintain-rfcs.png)<br /><br />
<br /><br />

1. Sroll down to the section **RFC - Standard Mode** and select the 3 check boxes.<br /><br />
![](../../images/b2-te2-maintain-rfcs-create-02.png)<br /><br />
<br /><br>

1. Scroll down to the section **Administration Users** and add the following credentials (same user for SAP Solution Manager TE2 and backend system TE2):
    * User: `SAP*`
    * Password: `Welcome18`<br /><br />
    ![](../../images/b2-te2-maintain-rfcs-admin-users.png)<br /><br />
<br /><br />

1. Then Scroll up and press the button **Execute**.<br /><br />
    ![](../../images/b2-te2-execute.png)<br /><br />

1. Confirm with **Yes** the upload of the roles to TE3.<br /><br />
![](../../images/b2-te2-maintain-rfcs-create-confirm.png)<br /><br />
<br /><br />

1. In the next popup, you will prompt to give the credentials of a superuser to upload the role. Enter the following details:
    * User: `SAP*`
    * Password: `Welcome18` <br /><br />
![](../../images/b2-te2-maintain-rfcs-create-confirm2.png)<br /><br />
<br /><br />

1. Press the **Save** button and go to Step 5: **Enter System Parameters**.<br /><br />
![](../../images/b2-te2-system-param.png)<br /><br />
<br /><br />

1. Go to **Common Parameters** and insert the following details:
    * Load Balancing Host: `wdflbmt7598.wdf.sap.corp`
    * Load Balancing Port: `8000`<br />
  and uncheck **Setup DBACockpit** in the **DB Parameters** section.<br /><br />
  ![](../../images/b2-te2-system-param2.png)<br /><br />
  <br /><br />

1. Save and go to step 7 **Finalize configuration**.
<br /><br />
![](../../images/b2-te2-finalize-config.png)<br /><br />

1. Go to the section **Automatic Activities**. Then select **Execute** in the dropdown list of **Activate e2e trace upload** and press the button **Execute Selected**.<br /><br />
![](../../images/be2-te2-finalize-config-execute-02.png)<br /><br />


## 2. Cloud services configuration

1. Before starting with configuration of the cloud service, let's add the SAP Cloud Platform certificate. Go to Chrome and open the URL `https://account.hanatrial.ondemand.com/` and logon. Then click on **Certificate** under **Secure**. (Be aware that the following procedure could be different if you use an other browser that Chrome).<br /><br />
![](../../images/b2-te2-cloud-services-cert.png)<br /><br />

1. In the popup, go to the **Details** tab and press the button **Copy to file**.<br /><br />
![](../../images/b2-te2-cloud-services-cert2.png)<br /><br />

1. Click **Next** for the first 2 steps and that click on **Browse**. Select **Desktop** and name the file `sapcp.cer` and click **Save**.<br /><br />
![](../../images/b2-te2-cloud-services-cert3.png)<br /><br />

1. Click again **Next** and **Finish** to download the certificate.<br /><br />
![](../../images/b2-te2-cloud-services-cert4.png)<br /><br />

1. Click on the favorite **Trust Manager** (Transaction STRUST).<br /><br />
![](../../images/b2-te2-cloud-services-cert-strust01.png)<br /><br />

1. Click the **Edit** icon and double-click on **SSL client SSL Client (Anonymous)** (Verify that you are on the right window ;). Then press the **Import** button.<br /><br />
![](../../images/b2-te2-cloud-services-cert-strust02.png)<br /><br />

1. Select your file **sapcp.cer** (that should saved on your desktop) and press the **Enter** button.<br /><br />
![](../../images/b2-te2-cloud-services-cert-strust03.png)<br /><br />

1. In the popup, click **Allow**.<br /><br />
![](../../images/b2-te2-cloud-services-cert-strust04.png)<br /><br />

1. Add the certificate as part of the trusted list by clicking on the button **Add to Certificate List** an finally press **Save**.<br /><br />
![](../../images/b2-te2-cloud-services-cert-strust05.png)<br /><br />

1. Go back to your browser tab with **Managed Systems Configuration** and press the button **Cloud Services**. If you closed the tab you can re-open it by ckicking again on the transaction favorite called **SAP Solution Manager Configurations** (Transaction SOLMAN_SETUP).<br /><br />
![](../../images/b2-te2-cloud-services.png)<br /><br />

1. Choose **Create Cloud Service** under **Cloud Services Operations**.<br /><br />
![](../../images/b2-te2-cloud-services-create.png)<br /><br />

1. In the wizard, select **SAP Cloud Platform** as service type and click **Next**.<br /><br />
![](../../images/b2-te2-cloud-services-type.png)<br /><br />

2. In the next step, give your SAP Cloud Platfform account name (e.g. p2000499901trial) and add a description for the cloud service.<br /><br />
![](../../images/b2-te2-cloud-services-definition.png)<br /><br />

1. Finally insert the Rool URL `https://publicapingplog.hanatrial.ondemand.com` as we are on the trial landscape. Click **Next** and in the last step, press **Finish**.<br /><br />
![](../../images/b2-te2-cloud-services-url.png)<br /><br />

    [//]: # (
    Add the URLs for the other landscapes and maybe the documentation URL...<br />
          https://support.sap.com/en/solution-manager/sap-solution-manager-7-2/expert-portal/applications/hybrid-operations/public-cloud-operations/sap-cloud-platform.html<br />
          https://publicapingplog.hana.ondemand.com<br />
          https://publicapingplog.hanatrial.ondemand.com<br />
          https://publicapingplog.neo.ondemand.com<br />
          )
<br /><br />

1. Now click on **Configure Cloud Service** to add the endpoint of the cloud service.<br /><br />
![](../../images/b2-te2-cloud-services-config.png)<br /><br />

1. In the new browser tab, press the button **Add** under the section **Cloud Service Endpoints**.<br /><br />
![](../../images/b2-te2-cloud-services-endpoint-add.png)<br /><br />

1. Insert the following details in the popup window:
    * Description: `SAP CP HTTP Endpoint`
    * User: `<YOUR-SUBACCOUNT-USERNAME>`(e.g. p2000499901)
    * Password: `Welcome18`
    * Proxy Host: `proxy`
    * Proxy Port: `8080`<br /><br />
  ![](../../images/b2-te2-cloud-services-endpoint-details.png)<br /><br />

1. Confirm the new endpoint by clicking on the **Save** button.<br /><br />
![](../../images/b2-te2-cloud-services-endpoint-save.png)<br /><br />

1. Click on the **Check** button to verify the configuration of the endpoint was successful.
<br /><br />
![](../../images/b2-te2-check-cloud-endpoint-02.png)


<br /><br /><br />

![](../../images/nav.png) [Previous exercise](../B1/README.md) ｜ [Next exercise](../B3/README.md) ｜ [Overview page](../../README.md)
