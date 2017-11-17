---
title: "GetTestSmtpConnectionResult Method"
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
ms.assetid: 933bdb86-7a0e-457d-826e-80c349744ab6searchScope: - ConfigMgr SDK
caps.latest.revision: 9
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# GetTestSmtpConnectionResult Method in Class SMS_Subscription
The `GetTestSmtpConnectionResult` Windows Management Instrumentation (WMI) class method, in System Center Configuration Manager, gets the test SMTP connection result.  

 The following syntax is simplified from Managed Object Format (MOF) code and defines the method.  

## Syntax  

```  
sint32 GetTestSmtpConnectionResult(  
     UInt32 TestID,  
     UInt32 ErrorCode  
);  
```  

#### Parameters  
 `TestID`  
 Data type: `UInt32`  

 Qualifiers: `[in]`  

 Test identifier returned by `TestSmtpConnection`.  

 `ErrorCode`  
 Data type: `UInt32`  

 Qualifiers: `[out]`  

 Represents the test results. Possible values are:  

|||  
|-|-|  
|0|Success.|  
|1|The test is initializing.|  
|2|Email address formatting error.|  
|3|Failed recipients error.|  
|4|Connection error.|  
|5|Other error.|  
|6|Operation timed out.|  

## Return Values  
 An  `SInt32` data type that is 0 to indicate success or non-zero to indicate failure.  

 For more information about handling returned errors, see [About Configuration Manager Errors](../../../../../develop/core/understand/about-configuration-manager-errors.md).  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../../../develop/core/reqs/server-development-requirements.md).  

## See Also  
 [SMS_Subscription Server WMI Class](../../../../../develop/reference/core/servers/manage/sms_subscription-server-wmi-class.md)   
 [Alert System WMI Server Classes](../../../../../develop/reference/core/servers/manage/alert-system-server-wmi-classes.md)
