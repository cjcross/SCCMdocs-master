---
title: "Deploy configuration baselines"
titleSuffix: "Configuration Manager"
description: "Deploy configuration baselines to define configuration baseline deployments and to add or remove configuration baselines from deployments."
ms.custom: na
ms.date: 10/06/2016
ms.prod: configuration-manager
ms.reviewer: na
ms.suite: na
ms.technology:
  - configmgr-other
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 9be8aaf3-075e-4acd-abd2-7459254e16e2
caps.latest.revision: 7
caps.handback.revision: 0
author: andredm7ms.author: andredmmanager: angrobe

---
# How to deploy configuration baselines in System Center Configuration Manager*Applies to: System Center Configuration Manager (Current Branch)*
Configuration baselines in System Center Configuration Manager must be deployed to one or more collections of users or devices before client devices in those collections can assess their compliance with the configuration baseline.  

Use the **Deploy Configuration Baselines** dialog box to define configuration baseline deployments, which includes adding or removing configuration baselines from deployments in addition to specifying the evaluation schedule.  

## Deploy a configuration baseline  

1.  In the Configuration Manager console, click **Assets and Compliance** > **Compliance Settings** > **Configuration Baselines**.  

3.  In the **Configuration Baselines** list, select the configuration baseline that you want to deploy, and then in the **Home** tab, in the **Deployment** group, click **Deploy**.  

4.  In the **Deploy Configuration Baselines** dialog box, select the configuration baselines that you want to deploy in the **Available configuration baselines** list. Click **Add** to add these to the **Selected configuration baselines** list.  

    > [!IMPORTANT]  
    >  If you change a configuration item that has been added to a deployed configuration baseline, the revised configuration item is not evaluated for compliance until its next scheduled evaluation time.  

5.  Specify the following additional information:  

    -   **Remediate noncompliant rules when supported** – Automatically remediates any rules that are noncompliant for Windows Management Instrumentation (WMI), the registry, scripts, and all settings for mobile devices that are enrolled by Configuration Manager.  

    -   **Allow remediation outside the maintenance window** – If a maintenance window has been configured for the collection to which you are deploying the configuration baseline, enable this option to let compliance settings remediate the value outside of the maintenance window. For more information about maintenance windows, see [How to use maintenance windows](/sccm/core/clients/manage/collections/use-maintenance-windows).  

6.  **Generate an alert** – Configures an alert that is generated if the configuration baseline compliance is less than a specified percentage by a specified date and time. You can also specify whether you want an alert to be sent to System Center Operations Manager.  

7.  **Collection** - Click **Browse** to select the collection where you want to deploy the configuration baseline.  

8.  **Specify the compliance evaluation schedule for this configuration baseline** Specifies the schedule by which the deployed configuration baseline is evaluated on client computers. This can be either a simple or a custom schedule.  

    > [!NOTE]  
    >  If the configuration baseline is deployed to a computer, it is evaluated for compliance within two hours of the start time that you schedule. If it is deployed to a user, it is evaluated for compliance when the user logs on.  

9. Click **OK** to close the **Deploy Configuration Baselines** dialog box and to create the deployment. For more information about how to monitor the deployment, see [Monitor compliance settings](/sccm/compliance/deploy-use/monitor-compliance-settings).  
