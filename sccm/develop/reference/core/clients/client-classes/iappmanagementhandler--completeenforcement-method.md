---
title: "IAppManagementHandler::CompleteEnforcement"
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
ms.assetid: bb69ca26-68de-4261-9ec8-42a732788d63searchScope: - ConfigMgr SDK
caps.latest.revision: 18
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# IAppManagementHandler::CompleteEnforcement Method
The `IAppManagementHandler::CompleteEnforcement` method, in Configuration Manager, completes the installation of a specific application. This method will be called only when the handler returned valid reconnection data in the EnforceApp call.  

## Syntax  

```  
[IDL]  
HRESULT CompleteEnforcement(  
     AppAction eEnforceAction,  
     IWbemClassObject* pHandlerSynclet,  
     IWbemClassObject* pReconnectData,  
     HANDLE hInstallProcess,  
     DWORD* pdwExitCode,  
     LPWSTR* ppszExecutionStatus  
);  
```  

#### Parameters  
 `eEnforceAction`  
 Data type: `AppAction`  

 Qualifiers: [in]  

 .   

 `pHandlerSynclet`  
 Data type: `IWbemClassObject`  

 Qualifiers: [in]  

 .   

 `pReconnectData`  
 Data type: `IWbemClassObject`  

 Qualifiers: [in]  

 .   

 `hInstallProcess`  
 Data type: `HANDLE`  

 Qualifiers: [in]  

 .   

 `pdwExitCode`  
 Data type: `DWORD`  

 Qualifiers: [out]  

 .   

 `ppszExecutionStatus`  
 Data type: `LPWSTR`  

 Qualifiers: [out]  

 .   

## Return Values  
 An `HRESULT` code. Possible values include, but are not limited to, the following:  

 S_OK  
 The method succeeded. All other return values indicate failure.  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Client Runtime Requirements](../../../../../develop/core/reqs/client-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Client Development Requirements](../../../../../develop/core/reqs/client-development-requirements.md).  

## See Also  
 [Application Management Client Interfaces](../../../../../develop/reference/core/clients/client-classes/application-management-client-interfaces.md)   
 [System Center Configuration Manager Software Development Kit](../../../../../develop/core/misc/system-center-configuration-manager-sdk.md)   
 [Scenario: Extending Application Management](../../../../../develop/apps/scenario--extending-application-management.md)   
 [Configuration Manager Reference](../../../../../develop/reference/configuration-manager-reference.md)
