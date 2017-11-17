---
title: "SMS_SofwareDistribution_Event"
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
ms.assetid: e382ccd4-fd11-4036-ad2a-a40397b86239searchScope: - ConfigMgr SDK
caps.latest.revision: 8
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# SMS_SofwareDistribution_Event
The `SMS_SofwareDistribution_Event` class is the base class for all software-distribution advertisement status-message classes, in Configuration Manager. All advertisement status messages have the insertion strings of this class. Also, each derived class must set the properties of its base `SMS_SofwareDistribution_Event` class.  

> [!NOTE]
>  The misspelling of software in `SMS_SofwareDistribution_Event` in this documentation is intentional as the implementation of the class is misspelled.  

## Properties  
 `AdvertisementId`  
 Data type: `String`  

 The Advertisement ID of the advertisement that the status message refers to. It appears in the status message text. It maps to the `ADV_AdvertisementID` field in the software distribution policy and to the Advertisement ID in the Configuration Manager console. This is insertion string number 1.  

 `ClientID`  
 Data type: `String`  

 The SMS identifier of the client raising this event.  

 `PackageName`  
 Data type: `String`  

 The Package ID that appears in the status message text. It maps to the `PKG_PackageID` field in the software distribution policy and to the Package ID in the Configuration Manager console. This is insertion string number 4.  

 `ProgramName`  
 Data type: `String`  

 The Program Name that appears in the status message text. It maps to the `PRG_ProgramName` field in the software distribution policy and is the program name that was chosen when the program was created. This is insertion string number 5.  

## See Also  
 [Status Message Types](../../../../../develop/reference/core/servers/manage/status-message-types.md)
