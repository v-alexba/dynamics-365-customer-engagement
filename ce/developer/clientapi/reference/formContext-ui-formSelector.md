---
title: "formContext.ui.FormSelector (Client API reference) in Dynamics 365 Customer Engagement| MicrosoftDocs"
description: "Learn about working with processes in Customer Engagement using client API."
ms.date: 10/31/2017
ms.service: "crm-online"
ms.topic: "reference"
applies_to: "Dynamics 365 (online)"
ms.assetid: 32e8d1d0-4093-4588-a517-2930eec34dce
author: "KumarVivek"
ms.author: "kvivek"
manager: "amyla"
---
# formContext.ui.formSelector (Client API reference)

[!INCLUDE[](../../../includes/cc_applies_to_update_9_0_0.md)]

The **formContext.ui.formSelector** property lets you work with form items where a form item represents a form that is available to a user because it is associated with a security role that the user is also associated to. Often there will be only one form. When more than one form is available, methods for a form item can be used to change the form the user is viewing.

Form Items are available through any of the following:

- **formselector.items** collection: A collection of all the form items accessible to the current user. Only those forms that share an association with one of the user’s security roles are available in this collection. Example:
 
    `formItem = formContext.ui.formSelector.items.get(arg);`

    See [Collections](collections.md)) for information about the collection methods.
 
    >[!NOTE]
    >This collection isn't available for Dynamics 365 mobile clients (phones and tablets).

- **formselector.getCurrentItem** method: Returns a reference to the form currently being shown. When only one form is available this method will return **null**. Example:
 
    `formItem = formContext.ui.formSelector.getCurrentItem();`       

## Form Item methods

After retrieving a form item using one of the above ways, use the following methods to work with the form item. 


|                        Name                         |                                                               Decription                                                               |
|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
|    [getId](formcontext-ui-formselector/getId.md)    |    [!INCLUDE[formcontext-ui-formselector/includes/getId-description.md](formcontext-ui-formselector/includes/getId-description.md)]    |
| [getLabel](formcontext-ui-formselector/getLabel.md) | [!INCLUDE[formcontext-ui-formselector/includes/getLabel-description.md](formcontext-ui-formselector/includes/getLabel-description.md)] |
| [navigate](formcontext-ui-formselector/navigate.md) | [!INCLUDE[formcontext-ui-formselector/includes/navigate-description.md](formcontext-ui-formselector/includes/navigate-description.md)] |

