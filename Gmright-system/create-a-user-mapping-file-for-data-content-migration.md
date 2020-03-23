---
title: "Create a user mapping file for data content migration"
ms.author: jhendr
author: JoanneHendrickson
manager: pamgreen
ms.date: 01/11/2018
ms.audience: ITPro
ms.topic: article
ms.prod: sharepoint-server-itpro
localization_priority: Priority
ms.collection: 
- IT_Sharepoint_Server_Top
- Strat_SP_gtc
ms.custom: 
ms.assetid: 28c42985-1fd6-49d6-b9c5-b7f35e83efa1
description: "This article describes how to create a user mapping file for data content migration while using the SharePoint Online Migration Tool."
---

# Create a user mapping file for data content migration

This article describes how to create a user mapping file for data content migration while using the SharePoint Online Migration Tool.
  
The SharePoint Migration Tool lets you migrate your files from SharePoint on-premises document libraries or your on-premises file shares and easily move them to either SharePoint or OneDrive in Office 365. It is available to Office 365 users.
  
> [!NOTE]
>  Currently the **SharePoint Migration Tool** is not available for users of Office 365 operated by 21Vianet in China. 
  
## Create a user mapping file for data content migration

When migrating your data from either a local file share or an on-premises SharePoint Server document library using the SharePoint Online Migration tool, a default user mapping file is used. You can also create your own using the following guidelines. Use any text editor, or an application like Excel, to create the CSV file.
  
 **CSV file format**
  
Here's an example of the format for the CSV file.
  
![User mapping file for data content migration](media/7ff2f07d-7e67-4834-974b-34651cc5e79f.jpg)
  
> [!IMPORTANT]
> Do not include a header row in your CSV file. 
  
 **To create a User Mapping file for data migration**
  
The following example uses Excel to create the CSV file.
  
1. Start Excel.
    
2. Enter the values for your user mapping.
    
  - **Column A:** Enter the **SID of the user** from the source location.  *Required.* 
    
  - **Column B:** Enter the **principal username** on the target site.  *Required.* 
    
  - **Column C:** If the principal username on the target site is a group, enter **TRUE**. If it is not a group, enter **FALSE**.  *Required.* 
    
3. Close and save as a Comma delimited (\*.csv) file.
    
 **Upload your User Mapping file to SharePoint Migration Tool**
  
After you create your own user mapping file, upload it to the SharePoint Online Migration tool.
  
1. Start the SharePoint Migration tool. Click **Next**. Enter your Office 365 username and password and then click **Sign in.**
    
2. Click the settings gear ![Settings for SPO Migration tool](media/bcec6d42-d9c4-4164-a8a3-456ca0eb6847.jpg) . 
    
3. In the User mapping box, click **Choose file** and select your user mapping file. 
    
4. Click **Save**.
    

