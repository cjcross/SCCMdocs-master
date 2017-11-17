---
title: "QueueAppPolicyActivationAction Method"
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
ms.assetid: 5c07606b-0f9f-4f1a-ae0f-2dfc2eaaab43searchScope: - ConfigMgr SDK
caps.latest.revision: 5
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# QueueAppPolicyActivationAction Method in Class CCM_RequestedAppPolicyActivation
The `QueueAppPolicyActivationAction` Windows Management Instrumentation (WMI) class method, in Configuration Manager, that queues an application policy activation action.   

 The following syntax is simplified from Managed Object Format (MOF) code and defines the method.  

## Syntax  

```  
uint32 QueueAppPolicyActivationAction   
{  
    [IN]    String PolicyId  
    [IN]    String PolicyRevision  
    [IN]    String Id  
    [IN]    UInt32 ActivationAction  
};  
```  

## Parameters  
 `PolicyId`  
 Data type: `String`  

 Qualifiers: [id("0"), in]  

 Policy identifier.    

 `PolicyRevision`  
 Data type: `String`  

 Qualifiers: [id("1"), in]  

 Policy revision.    

 `Id`  
 Data type: `String`  

 Qualifiers: [id("2"), in]  

 Application identifier.    

 `ActivationAction`  
 Data type: `UInt32`  

 Qualifiers: [id("3"), in]  

 Activation action. Possible values are:  

|||  
|-|-|  
|0|default|  
|1|By-pass activation.|  

## Remarks  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../../../develop/core/reqs/server-development-requirements.md).
