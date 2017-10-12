---
title: "Microsoft Dynamics 365 Customer Engagement subscriptionsyncentryoffline EntityType Reference | MicrosoftDocs"
ms.date: 07/10/2017
ms.service: "crm-online"
ms.topic: "reference"
applies_to: 
  - "Dynamics 365 (online)"
ms.assetid: 46f9d85f-e1fb-4e58-9889-62e41c6fb090
author: "jimdaly"
ms.author: "jdaly"
manager: "jdaly"
meta-description: "Reference information about the Web API subscriptionsyncentryoffline entitytype."
---
# subscriptionsyncentryoffline EntityType
<table>
<tr><td><b>Description:</b></td><td>[!INCLUDE[./descriptions/subscriptionsyncentryoffline.md](./descriptions/subscriptionsyncentryoffline.md)]</td></tr>
<tr><td><b>Entity Set path:</b></td><td>[!include[current-web-api-base-uri.md](../includes/current-web-api-base-uri.md)]subscriptionsyncentriesoffline </td></tr>
<tr><td><b>Base Type:</b></td><td>[crmbaseentity EntityType](crmbaseentity.md)</td></tr>
<tr><td><b>Display Name:</b></td><td>Subscription Sync Entry Offline</td></tr>
<tr><td><b>Primary Key:</b></td><td>subscriptionid</td></tr>
<tr><td><b>Primary Name Attribute:</b></td><td>None</td></tr>
<tr><td><b>Operations supported:</b></td><td>None</td></tr>
</table>
  
The subscriptionsyncentryoffline EntityType:
* Has no lookup properties.
* Has no single-valued navigation properties.
* Has no collection-valued navigation properties.
* Has no functions or actions bound to it.
* Is not included in any solutions.

## Properties
Properties represent fields of data stored in the entity. Some properties are read-only. 


|Name|Type|Details|  
|----|----|-------|  
|objectid|Edm.Guid|**Display Name**: ObjectId<br />**Description**: Object Id<br />|
|objecttypecode|Edm.Int32|**Display Name**: ObjectTypeCode<br />**Description**: Entity object type code<br />|
|subscriptionid|Edm.Guid|**Display Name**: SubscriptionId<br />**Description**: Subscription Id<br />|
|syncstate|Edm.Int32|**Display Name**: SyncState<br />**Description**: Sync state<br />|
|versionnumber|Edm.Int64|**Display Name**: VersionNumber<br />**Description**: Version number<br />|  

[!INCLUDE[./remarks/subscriptionsyncentryoffline.md](./remarks/subscriptionsyncentryoffline.md)]

### See also  
 [Use the Microsoft Dynamics CRM Web API](https://msdn.microsoft.com/library/mt593051.aspx)<br />
 [Web API EntityType Reference](../entitytypereference.md)<br />
 [Web API Action Reference](../actionreference.md)<br />
 [Web API Function Reference](../functionreference.md)<br />
 [Web API Query Function Reference](../queryfunctionreference.md)<br />
 [Web API EnumType Reference](../enumtypereference.md)<br />
 [Web API ComplexType Reference](../complextypereference.md)<br />
 [Web API Metadata EntityType Reference](../entitytypereference.md)<br />
 [Web API Solutions Reference](../solutionreference.md)<br />