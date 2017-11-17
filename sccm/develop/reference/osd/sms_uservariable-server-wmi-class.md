---
title: "SMS_UserVariable Class"
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
ms.assetid: aaeefdd5-32ac-4b17-ad1d-fd9cb50b9ae0searchScope: - ConfigMgr SDK
caps.latest.revision: 9
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# SMS_UserVariable Server WMI Class
The `SMS_UserVariable` Windows Management Instrumentation (WMI) class is an SMS Provider server class, in Configuration Manager, that defines the settings of a specific user (such as IsCloudUser=True/False).  

 The following syntax is simplified from Managed Object Format (MOF) code and includes all inherited properties.  

## Syntax  

```  
Class SMS_UserVariable  
{  
      Boolean IsMasked;  
      String Name;  
      String Value;  
};  
```  

## Methods  
 The `SMS_UserVariable` class does not define any methods.  

## Properties  
 `IsMasked`  
 Data type: `Boolean`  

 Access type: Read/Write  

 Qualifiers: None  

 This property is not currently used.  

 `Name`  
 Data type: `String`  

 Access type: Read/Write  

 Qualifiers: [key]  

 The name of the user variable. The default value is "".  

 `Value`  
 Data type: `String`  

 Access type: Read/Write  

 Qualifiers: None  

 The user variable value. The default value is `null`.  

## Remarks  
 Class qualifiers for this class include:  

-   Embedded  

 For more information about both the class qualifiers and the property qualifiers that are included in the Properties section, see [Configuration Manager Class and Property Qualifiers](../../../develop/reference/misc/class-and-property-qualifiers.md).  

 Your application uses this class to create objects that are embedded by the SMS_UserSettings Server WMI Class and accessed by using the `UserVariables` property.  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../develop/core/reqs/server-development-requirements.md).  

## See Also  
 [Operating System Deployment Server WMI Classes](../../../develop/reference/osd/operating-system-deployment-server-wmi-classes.md)   
 [SMS_CollectionVariable Server WMI Class](../../../develop/reference/osd/sms_collectionvariable-server-wmi-class.md)
