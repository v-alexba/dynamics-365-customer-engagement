---
title: "NextXFiscalYears Query Function | MicrosoftDocs"
ms.date: 07/10/2017
ms.service: "crm-online"
ms.topic: "reference"
applies_to: 
  - "Dynamics 365 (online)"
ms.assetid: 23dad51d-5b49-469e-897c-6b5551231efb
author: "jimdaly"
ms.author: "jdaly"
manager: "jdaly"
---
# NextXFiscalYears Function
[!INCLUDE[./descriptions/nextxfiscalyears.md](./descriptions/nextxfiscalyears.md)]  
  
|Name|Type|Nullable|Unicode|Description|  
|----------|----------|--------------|-------------|-----------------|  
|PropertyName|Edm.String|false|false|The name of the property to evaluate. |
|PropertyValue|Edm.Int64|false|true|The value to compare. | 


## Syntax example
`?$filter=Microsoft.Dynamics.CRM.NextXFiscalYears(PropertyName=@p1,PropertyValue=@p2)&@p1='name'&@p2=42`
 
[!INCLUDE[./remarks/nextxfiscalyears.md](./remarks/nextxfiscalyears.md)]

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