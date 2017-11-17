---
title: "SMS_SummarizationInterval Class"
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
ms.assetid: bab2b232-fde6-4127-9e13-5f496e385447searchScope: - ConfigMgr SDK
caps.latest.revision: 8
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# SMS_SummarizationInterval Server WMI Class
The `SMS_SummarizationInterval` Windows Management Instrumentation (WMI) class is an SMS Provider server class, in System Center Configuration Manager, that represents the months that have been summarized by a monthly usage summary.  

 The following syntax is simplified from Managed Object Format (MOF) code and includes all inherited properties.  

## Syntax  

```  
Class SMS_SummarizationInterval : SMS_BaseClass  
{  
      DateTime IntervalStart;  
      UInt32 TimeKey;  
};  
```  

## Methods  
 The `SMS_SummarizationInterval` class does not define any methods.  

## Properties  
 `IntervalStart`  
 Data type: `DateTime`  

 Access type: Read/Write  

 Qualifiers: None  

 Date and time when the software metering interval starts.  

 `TimeKey`  
 Data type: `UInt32`  

 Access type: Read/Write  

 Qualifiers: [key]  

 Key that uniquely identifies the interval, equivalent to 100*Year+Month.  

## Remarks  
 There are no special class qualifiers for this class. For more information about both the class qualifiers and the property qualifiers included in the Properties section, see [Configuration Manager Class and Property Qualifiers](../../../develop/reference/misc/class-and-property-qualifiers.md).  

 This class is the source for the `TimeKey` property in a monthly usage summary represented by [SMS_MonthlyUsageSummary Server WMI Class](../../../develop/reference/apps/sms_monthlyusagesummary-server-wmi-class.md).  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../develop/core/reqs/server-development-requirements.md).  

## See Also  
 [Software Metering Server WMI Classes](../../../develop/reference/apps/software-metering-server-wmi-classes.md)   
 [SMS_MonthlyUsageSummary Server WMI Class](../../../develop/reference/apps/sms_monthlyusagesummary-server-wmi-class.md)
