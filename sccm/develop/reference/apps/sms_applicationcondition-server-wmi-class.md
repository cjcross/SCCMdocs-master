---
title: "SMS_ApplicationCondition Class"
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
ms.assetid: 4d92732b-9f97-42fe-a441-559a87f05588searchScope: - ConfigMgr SDK
caps.latest.revision: 6
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# SMS_ApplicationCondition Server WMI Class
The `SMS_ApplicationCondition` Windows Management Instrumentation (WMI) class is an SMS Provider server class, in Configuration Manager, that represents relationships between global conditions and applications.  

 The following syntax is simplified from Managed Object Format (MOF) code and includes all inherited properties.  

## Syntax  

```  
Class SMS_ApplicationCondition : SMS_BaseClass  
{  
    String ApplicationGUID;  
    String ConditionDisplayName;  
    UInt32 ConditionID;  
    String ConditionModelName;  
};  
```  

## Methods  
 The `SMS_ApplicationCondition` class does not define any methods.  

## Properties  
 `ApplicationGUID`  
 Data type: `String`  

 Access type: Read-only  

 Qualifiers: [not_null, read]  

 Unique identifier of the application.  

 `ConditionDisplayName`  
 Data type: `String`  

 Access type: Read-only  

 Qualifiers: [read]  

 Condition display name.  

 `ConditionID`  
 Data type: `UInt32`  

 Access type: Read-only  

 Qualifiers: [not_null, read]  

 Identifier of the application condition.  

 `ConditionModelName`  
 Data type: `String`  

 Access type: Read-only  

 Qualifiers: [not_null, read]  

 Model name of the condition.  

## Remarks  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../develop/core/reqs/server-development-requirements.md).  

## See Also  
 [Configuration Manager Content Server WMI Classes](../../../develop/reference/core/servers/configure/content-server-wmi-classes.md)
