---
title: "SMS_SecondarySiteStatus Class"
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
ms.assetid: fc28e42f-09f5-41aa-870a-28a673dfe6bcsearchScope: - ConfigMgr SDK
caps.latest.revision: 6
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# SMS_SecondarySiteStatus Server WMI Class
The `SMS_SecondarySiteStatus` Windows Management Instrumentation (WMI) class is an SMS Provider server class, in Configuration Manager, that represents secondary site installation or uninstallation status.  

 The following syntax is simplified from Managed Object Format (MOF) code and includes all inherited properties.  

## Syntax  

```  
Class SMS_SecondarySiteStatus : SMS_BaseClass  
{  
    String Description;  
    DateTime MessageTime;  
    String SiteCode;  
    UInt32 SiteInstallID;  
    String Status;  
    UInt32 StatusID;  
};  
```  

## Methods  
 The `SMS_SecondarySiteStatus` class does not define any methods.  

## Properties  
 `Description`  
 Data type: `String`  

 Access type: Read  

 Qualifiers: none  

 Description of the status for secondary installation or uninstallation status.  

 `MessageTime`  
 Data type: `DateTime`  

 Access type: Read  

 Qualifiers: [key]  

 Time of the message reported for the secondary site installation or uninstallation.  

 `SiteCode`  
 Data type: `String`  

 Access type: Read  

 Qualifiers: [key]  

 Site code of the secondary site.  

 `SiteInstallID`  
 Data type: `UInt32`  

 Access type: Read  

 Qualifiers: [key]  

 Site installation or uninstallation identifier.  

 `Status`  
 Data type: `String`  

 Access type: Read  

 Qualifiers: none  

 Secondary site installation or uninstallation status.  

 `StatusID`  
 Data type: `UInt32`  

 Access type: Read  

 Qualifiers: [key]  

 Identifier for the status.  

## Remarks  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../../../develop/core/reqs/server-development-requirements.md).  

## See Also  
 [Status Server WMI Classes](../../../../../develop/reference/core/servers/manage/status-server-wmi-classes.md)
