---
title: "Introduction to power management"
titleSuffix: "Configuration Manager"
description: "Get an introduction to power management in System Center Configuration Manager."
ms.custom: na
ms.date: 10/06/2016
ms.prod: configuration-manager
ms.reviewer: na
ms.suite: na
ms.technology:
  - configmgr-other
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 3ddff2a7-99eb-4ef8-b969-f3f7f24053db
caps.latest.revision: 4
caps.handback.revision: 0
author: arob98

---
# Introduction to power management in System Center Configuration Manager
Power Management in System Center Configuration Manager addresses the need that many organizations have to monitor and reduce the power consumption of their computers. The feature takes advantage of the power management features built into Windows to apply relevant and consistent settings to computers in the organization. You can apply different power settings to computers during business hours and nonbusiness hours. For example, you might want to apply a more restrictive power plan to computers during nonbusiness hours. In cases where computers must always remain turned on, you can prevent power management settings from being applied.  

 Power management in Configuration Manager includes several reports to help you analyze power consumption and computer power settings in your organization. You can also use the reports to help you troubleshoot problems with power management.  

 For a detailed workflow about how to configure and use power management, see [Administrator checklist for power management in System Center Configuration Manager](../../../../core/clients/manage/power/administrator-checklist-for-power-management.md).  

> [!IMPORTANT]  
>  Configuration Manager power management is not supported on virtual machines. You cannot apply power plans to virtual machines, nor can you or report power data from them.  

## The power management workflow  
 Use the following three phases to plan and implement power management in Configuration Manager.  

### Monitoring and planning phase  
 Power Management uses Configuration Manager hardware inventory to collect data about computer usage and power settings for computers in the site. There are a number of reports that you can use to analyze this data and determine the optimal power management settings for computers. For example, during the monitoring and planning phase of the power management workflow, you can create collections that are based on the data that is included in the **Power Capabilities** report and use that data to identify the computers that are not capable of power management. Then, you can exclude those computers from power management.  

> [!IMPORTANT]  
>  Do not apply power plans to computers in your site until you collect and analyze the power data from client computers. If you apply new power management settings to computers without first examining the existing settings, you might experience an increase in power consumption.  

### Enforcement phase  
 Power management lets you create power plans that you can apply to collections of computers in your site. These power plans configure Windows power management settings on computers. You can use the power plans that are included with Configuration Manager, or you can configure your own custom power plans. You can use the power data that is collected during the monitoring and planning phase as a baseline to help you evaluate power savings after you apply a power plan to computers. For more information, see [Administrator checklist for power management in System Center Configuration Manager](../../../../core/clients/manage/power/administrator-checklist-for-power-management.md).  

### Compliance phase  
 In the compliance phase, you can run reports that help you to evaluate power usage and power cost savings in your organization. You can also run reports that describe the improvements in the amount of CO2 generated by computers. Reports are also available that help you validate that power settings were correctly applied to computers and that help you troubleshoot problems with the power management feature.  