---
title: "SMS_SUPSyncStatus Class"
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
ms.assetid: 2ed724a6-b660-4d71-9580-901814bec745searchScope: - ConfigMgr SDK
caps.latest.revision: 11
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# SMS_SUPSyncStatus Server WMI Class
The `SMS_SUPSyncStatus` Windows Management Instrumentation (WMI) class is an SMS Provider server class, in System Center Configuration Manager, that lists sync and replication status for SUM data for participating site/SUP.  

 The following syntax is simplified from Managed Object Format (MOF) code and includes all inherited properties.  

## Syntax  

```  
Class SMS_SUPSyncStatus : SMS_BaseClass  
{  
    DateTime LastReplicationLinkCheckTime;  
    DateTime LastSuccessfulSyncTime;  
    UInt32 LastSyncErrorCode;  
    UInt32 LastSyncState;  
    DateTime LastSyncStateTime;  
    UInt32 ReplicationLinkStatus;  
    String SiteCode;  
    UInt32 SyncCatalogVersion;  
    String WSUSServerName;  
    String WSUSSourceServer;  
};  
```  

## Methods  
 The `SMS_SUPSyncStatus` class does not define any methods.  

## Properties  
 `LastReplicationLinkCheckTime`  
 Data type: `DateTime`  

 Access type: Read-only  

 Qualifiers: [read]  

 Last time the replication link status was checked.  

 `LastSuccessfulSyncTime`  
 Data type: `DateTime`  

 Access type: Read-only  

 Qualifiers: [read]  

 Last synchronization success time.  

 `LastSyncErrorCode`  
 Data type: `UInt32`  

 Access type: Read-only  

 Qualifiers: [not_null, read]  

 Last synchronization error code.  

 `LastSyncState`  
 Data type: `UInt32`  

 Access type: Read-only  

 Qualifiers: [read]  

 Last synchronization state.  

 `LastSyncStateTime`  
 Data type: `DateTime`  

 Access type: Read-only  

 Qualifiers: [read]  

 Last time the synchronization state was reported.  

 `ReplicationLinkStatus`  
 Data type: `UInt32`  

 Access type: Read-only  

 Qualifiers: [enumeration, read]  

 Replication link status.  

|||  
|-|-|  
|0|Healthy|  
|1|Degraded|  
|2|Error|  

 `SiteCode`  
 Data type: `String`  

 Access type: Read-only  

 Qualifiers: [key, not_null, read]  

 Site code.  

 `SyncCatalogVersion`  
 Data type: `UInt32`  

 Access type: Read-only  

 Qualifiers: [read]  

 Synchronization catalog version.  

 `WSUSServerName`  
 Data type: `String`  

 Access type: Read-only  

 Qualifiers: [key, not_null, read]  

 WSUS server name.  

 `WSUSSourceServer`  
 Data type: `String`  

 Access type: Read-only  

 Qualifiers: [not_null, read]  

 WSUS source server.  

## Remarks  

## Requirements  

## Runtime Requirements  
 For more information, see [Configuration Manager Server Runtime Requirements](../../../develop/core/reqs/server-runtime-requirements.md).  

## Development Requirements  
 For more information, see [Configuration Manager Server Development Requirements](../../../develop/core/reqs/server-development-requirements.md).  

## See Also  
 [Software Updates Server WMI Classes](../../../develop/reference/sum/software-updates-server-wmi-classes.md)   
 [Configuration Manager Software Updates](../../../develop/sum/software-updates.md)
