---
title: "Delete a Package"
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
ms.assetid: 0ca0c411-c33e-444b-a96c-4279042fcda4searchScope: - ConfigMgr SDK
caps.latest.revision: 10
author: "shill-ms"
ms.author: "v-suhill"
manager: "mbaldwin"
---
# How to Delete a Package
The following example shows how to delete a package in System Center Configuration Manager by using the `SMS_Package` class.  

> [!NOTE]
>  Any reference to this package, such as an advertisement or task sequence, should be cleaned up before deleting the package  

### To delete a package  

1.  Set up a connection to the SMS Provider.  

2.  Load the existing package object by using the `SMS_Package` class.  

3.  Delete the package by using the delete method.  

## Example  
 The following example method deletes an existing package.  

 For information about calling the sample code, see [Calling Configuration Manager Code Snippets](../../../../develop/core/understand/calling-code-snippets.md).  

```vbs  

Sub DeleteAPackage(connection, existingPackageID)  

    ' Get the specified package instance (passed in as existingPackageID).    Dim packageToDelete  
    Set packageToDelete = connection.Get("SMS_Package.PackageID='" & existingPackageID & "'")  

    ' Delete the package.  
    PackageToDelete.Delete_  

    ' Output package ID of deleted package.  
    wscript.echo "Deleted Package ID: " & existingPackageID  

End Sub  
```  

```c#  
public void DeleteAPackage(WqlConnectionManager connection, string existingPackageID)  
{  
    try  
    {  
        // Get the specified package instance (passed in as existingPackageID).  
        IResultObject packageToDelete = connection.GetInstance(@"SMS_Package.PackageID='" + existingPackageID + "'");  

        // Delete the package instance.  
        packageToDelete.Delete();  

        // Output package ID of deleted package.  
        Console.WriteLine("Deleted Package ID: " + existingPackageID);  
    }  

    catch (SmsException ex)  
    {  
        Console.WriteLine("Failed to create package. Error: " + ex.Message);  
        throw;  
    }  
}  
```  

 The example method has the following parameters:  

|Parameter|Type|Description|  
|---------------|----------|-----------------|  
|`connection`<br /><br /> `swbemServices`|-   Managed: `WqlConnectionManager`<br />-   VBScript: [SWbemServices](https://msdn.microsoft.com/library/aa393854.aspx)|A valid connection to the SMS Provider.|  
|`existingPackageID`|-   Managed: `String`<br />-   VBScript: `String`|The ID of the existing package.|  

## Compiling the Code  
 The C# example requires:  

### Namespaces  
 System  

 Microsoft.ConfigurationManagement.ManagementProvider  

 Microsoft.ConfigurationManagement.ManagementProvider.WqlQueryEngine  

### Assembly  
 adminui.wqlqueryengine  

 microsoft.configurationmanagement.managementprovider  

 mscorlib  

## Robust Programming  
 For more information about error handling, see [About Configuration Manager Errors](../../../../develop/core/understand/about-configuration-manager-errors.md).  

## .NET Framework Security  

## See Also  
 [Configuration Manager Software Distribution](../../../../develop/core/servers/configure/software-distribution.md)   
 [Software Distribution Packages](../../../../develop/core/servers/configure/software-distribution-packages.md)   
 [SMS_SCI_Component Server WMI Class](../../../../develop/reference/core/servers/configure/sms_sci_component-server-wmi-class.md)
