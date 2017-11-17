---
title: "ITsMediaClass::CurrentStep Property"
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
ms.assetid: adb0a5f9-0880-483a-aa87-ea9dba926125searchScope: - ConfigMgr SDK
caps.latest.revision: 6
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# ITsMediaClass::CurrentStep Property
Iin Configuration Manager, the `CurrentStep` property contains the current step in asynchronous task sequence media creation.  

## Syntax  

```  
[IDL]  
HRESULT SiteCode([out,retval] long* Step);  
```  

#### Parameters  
 `Step`  
 Data type: `long`  

 Qualifiers: [out, retval]  

 Pointer to the current step.  

## Return Values  
 An `HRESULT` code. Possible values include, but are not limited to, the following value.  

 S_OK  
 The method succeeded.  

## Remarks  
 You can use the `CurrentStep` property in conjunction with [ITsMediaClass::NumSteps Property](../../../develop/reference/misc/itsmediaclass--numsteps-property.md) to estimate the overall progress of media creation.  

## See Also  
 [ITsMediaClass Interface](../../../develop/reference/misc/itsmediaclass-interface.md)   
 [ITsMediaClass::NumSteps Property](../../../develop/reference/misc/itsmediaclass--numsteps-property.md)
