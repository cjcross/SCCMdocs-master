---
title: "ITsMediaClass::SiteCode Property"
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
ms.assetid: bf39ba0f-1c28-4fe3-a757-1d342b1415cbsearchScope: - ConfigMgr SDK
caps.latest.revision: 6
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# ITsMediaClass::SiteCode Property
In Configuration Manager, the `SiteCode` property contains the site code for the site server.  

## Syntax  

```  
[IDL]  
HRESULT SiteCode([in] BSTR SiteCode);  

HRESULT SiteCode([out,retval] BSTR* SiteCode);  
```  

#### Parameters  
 `SiteCode`  
 Data type: `BSTR`  

 Qualifiers: [in; out, retval]  

 On input, the site code to set. On output, this parameter points to the retrieved site code.  

## Return Values  
 An `HRESULT` code. Possible values include, but are not limited to, the following value.  

 S_OK  
 The method succeeded.  

## Remarks  

## See Also  
 [ITsMediaClass Interface](../../../develop/reference/misc/itsmediaclass-interface.md)
