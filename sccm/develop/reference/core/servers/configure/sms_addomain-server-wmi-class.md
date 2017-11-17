---
title: "SMS_ADDomain Class"
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
ms.assetid: 11409ed9-d32c-4d0f-abc8-1fee24641377searchScope: - ConfigMgr SDK
caps.latest.revision: 9
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# SMS_ADDomain Server WMI Class
The `SMS_ADDomain` Windows Management Instrumentation (WMI) class is an SMS Provider server class, in Configuration Manager, that contains Active Directory domains discovered by Configuration Manager Forest Discovery.  

 The following syntax is simplified from Managed Object Format (MOF) code and includes all inherited properties.  

## Syntax  

```  
Class SMS_ADDomain : SMS_BaseClass  
{  
    UInt32 DomainID;  
    String DomainMode;  
    String DomainName;  
    UInt32 Flags;  
    UInt32 ForestID;  
    DateTime LastDiscoveryTime;  
};  
```  

## Methods  
 The `SMS_ADDomain` class does not define any methods.  

## Properties  
 `DomainID`  
 Data type: `UInt32`  

 Access type: Read/Write  

 Qualifiers: [key]  

 Identifier of the Active Directory domain.  

 `DomainMode`  
 Data type: `String`  

 Access type: Read-only  

 Qualifiers: [read]  

 The functional level of the Active Directory forest.  

|Forest Functional Level|  
|-----------------------------|  
|Windows 2000|  
|Windows Server 2003 interim|  
|Windows Server 2003|  
|Windows Server 2008|  
|Windows Server 2008 R2|  

 `DomainName`  
 Data type: `String`  

 Access type: Read-only  

 Qualifiers: [read]  

 The name of the Active Directory domain.  

 `Flags`  
 Data type: `UInt32`  

 Access type: Read-only  

 Qualifiers: [read]  

 Flags.   

 `ForestID`  
 Data type: `UInt32`  

 Access type: Read/Write  

 Qualifiers: [key]  

 The identifier of Active Directory forest.  

 `LastDiscoveryTime`  
 Data type: `DateTime`  

 Access type: Read-only  

 Qualifiers: [read]  

 The last time this domain was discovered by Active Directory forest discovery.  

## Remarks  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../../../develop/core/reqs/server-development-requirements.md).  

## See Also  
 [Discovery Server WMI Classes](../../../../../develop/reference/core/servers/configure/discovery-server-wmi-classes.md)
