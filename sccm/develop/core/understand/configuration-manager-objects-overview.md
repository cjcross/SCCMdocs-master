---
title: "Objects Overview"
titleSuffix: "Configuration Manager"
ms.custom: ""
ms.date: "09/20/2016"
ms.prod: "configuration-manager"
ms.reviewer: ""
ms.suite: ""
ms.technology:
  - "configmgr-other"
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to:
  - "System Center Configuration Manager (current branch)"
ms.assetid: f3ddf4dc-2acd-4d59-be88-b2296d9333cdsearchScope: - ConfigMgr SDK
caps.latest.revision: 7
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# Configuration Manager Objects Overview
The System Center Configuration Manager objects are instances of Configuration Manager-specific Windows Management Instrumentation (WMI) classes that are managed by the SMS Provider. The Configuration Manager object class categories are described in the following table.  

|System Center Configuration Manager Object Class Category|Description|  
|----------------------------------------------------------------------------------------|-----------------|  
|Software distribution|Objects associated with the software distribution feature of Configuration Manager, such as advertisement, collection, package, and program objects.|  
|Scheduling|Organizes scheduled Configuration Manager events, such as inventory updates.|  
|Site|Contains information about Configuration Manager sites.|  
|Security|Describes the permissions granted to users and user groups to operate on specific Configuration Manager-secured objects, such as program and package objects.|  
|Query|Describes Configuration Manager site database queries.|  
|Resource|Populated when Configuration Manager discovers potential client computers, users, user groups, and other types of objects within the boundaries of the site.|  
|Inventory|Provides the structure for inventory operations on Configuration Manager client systems, users, and user groups.|  
|Software metering|Describes the metered Configuration Manager resources, such as program files.|  
|Status and summarizer|Indicates the status of Configuration Manager sites, components, and software distribution operations.|  
|Collected files|Contains information about files collected from clients.|  

## DebugView  
 To show SMS Provider object property values in the System Center Configuration Manager console results pane, start the console with the following command line:  

 \<InstallationDirectory>\Microsoft.ConfigurationManagement.exe /SMS:DebugView=1  

 For more information about command-line options, see [Configuration Manager Console Command-Line Options](../../../develop/reference/core/servers/console/console-command-line-options.md)  

## See Also  
 [Configuration Manager Association Classes](../../../develop/core/understand/association-classes.md)   
 [Configuration Manager Bit Field Properties](../../../develop/core/understand/configuration-manager-bit-field-properties.md)   
 [Configuration Manager Console Command-Line Options](../../../develop/reference/core/servers/console/console-command-line-options.md)   
 [Configuration Manager Date and Time Formats](../../../develop/core/understand/date-and-time-formats.md)   
 [Configuration Manager Embedded Objects](../../../develop/core/understand/embedded-objects.md)   
 [Configuration Manager Extended WMI Query Language](../../../develop/core/understand/extended-wmi-query-language.md)   
 [How to Use Configuration Manager Objects With Managed Code](../../../develop/core/understand/how-to-use-configuration-manager-objects-with-managed-code.md)   
 [Configuration Manager Lazy Properties](../../../develop/core/understand/configuration-manager-lazy-properties.md)   
 [Configuration Manager Errors](../../../develop/core/understand/configuration-manager-errors.md)   
 [Configuration Manager Object Security](../../../develop/core/understand/configuration-manager-object-security.md)   
 [Configuration Manager Special Queries](../../../develop/core/understand/special-queries.md)
