---
title: "CCM_RequestedAppPolicyActivation Class"
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
ms.assetid: 9453f2e6-006a-4932-b67f-fda5e149133asearchScope: - ConfigMgr SDK
caps.latest.revision: 11
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# CCM_RequestedAppPolicyActivation Client WMI Class
The `CCM_RequestedAppPolicyActivation` Windows Management Instrumentation (WMI) class is an SMS Provider server class, in Configuration Manager, that represents a requested application policy activation.  

 The following syntax is simplified from Managed Object Format (MOF) code and includes all inherited properties.  

## Syntax  

```  
Class CCM_RequestedAppPolicyActivation :    
{  
    UInt32 ActivationAction;  
    String AppId;  
    DateTime DateRequested;  
    Boolean IsComplete;  
    String PolicyId;  
    String Revision;  
    String UserSID;  
};  
```  

## Methods  
 The following table lists the methods in the `CCM_RequestedAppPolicyActivation` class.  

-   [QueueAppPolicyActivationAction Method in Class CCM_RequestedAppPolicyActivation](../../../../../develop/reference/core/clients/sdk/queueapppolicyactivationaction-method-in-class-ccm_requestedapppolicyactivation.md)  

## Properties  
 `ActivationAction`  
 Data type: `UInt32`  

 Access type: Read/Write  

 Qualifiers: [values]  

 Activation action. Possible value are:  

|||  
|-|-|  
|0|default|  
|1|By-pass Activation|  

 `AppId`  
 Data type: `String`  

 Access type: Read/Write  

 Qualifiers: none  

 Application identifier.    

 `DateRequested`  
 Data type: `DateTime`  

 Access type: Read/Write  

 Qualifiers: none  

 Date requested.    

 `IsComplete`  
 Data type: `Boolean`  

 Access type: Read/Write  

 Qualifiers: none  

 `true` if activation is complete.    

 `PolicyId`  
 Data type: `String`  

 Access type: Read/Write  

 Qualifiers: [key]  

 Policy identifier.    

 `Revision`  
 Data type: `String`  

 Access type: Read/Write  

 Qualifiers: none  

 Application revision.    

 `UserSID`  
 Data type: `String`  

 Access type: Read/Write  

 Qualifiers: [key]  

 User security identifier (SID).    

## Remarks  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../../../develop/core/reqs/server-development-requirements.md).  

## See Also  
 [Configuration Manager Client SDK WMI Classes](../../../../../develop/reference/core/clients/sdk/client-sdk-wmi-classes.md)
