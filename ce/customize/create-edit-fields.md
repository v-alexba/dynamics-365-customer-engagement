---
title: "Create and edit fields (Dynamics 365 Customer Engagement) | MicrosoftDocs"
ms.custom: ""
ms.date: 09/30/2017
ms.reviewer: ""
ms.service: "crm-online"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to: 
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
ms.assetid: d88677fa-2caf-47b0-aec6-10a25a7ec9c3
caps.latest.revision: 55
ms.author: "rdubois"
manager: "brycho"
---
# Create and edit fields (attributes)

[!INCLUDE[cc-applies-to-update-9-0-0](../includes/cc_applies_to_update_9_0_0.md)]

In [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)], fields define the individual data items that can be used to store data in an entity. Fields are sometimes called attributes by developers. You can use the customization tools in the solution explorer to edit system fields that allow customization, or to create, edit, or delete custom entities.  
  
<a name="BKMK_CreatingAndEditngFields"></a>   
## Create and edit fields  
 Before you create a custom field, evaluate whether using an existing field meets your requirements. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Create new metadata or use existing metadata](../customize/create-edit-metadata.md#BKMK_CreateNewOrUseExistingMetadata)  
  
 Part of the name of any custom field you create is the customization prefix. This is set based on the solution publisher for the solution you’re working in. If you care about the customization prefix, make sure that you are working in an unmanaged solution or the default solution where the customization prefix is the one you want for this entity. For information about how to change the customization prefix, see [Solution Publisher](../customize/change-solution-publisher-prefix.md#BKMK_SolutionPublisher).  
  
 You can access fields in the application in several ways:  
  
-   From the solution explorer you can expand the entity and choose the **Fields** node. From the list of fields, click **New** to create a new field or double-click any of the fields on the list to edit them.  
  
-   Expand the entity and choose the **Forms** node. Open a form in the form editor and below the **Field Explorer** click **New Field** to create a new field. For any field already added to the form you can double-click the field to display the **Field Properties**. On the **Details** tab, click **Edit**. Another way to go  to the form editor is to use the **Form** command on the command bar for any entity record.  
  
-   If you use the metadata browser tool, use the **Entity Metadata Browser** page to view details about a specific entity, and then click the **Attributes** button. If a field is editable, you can click the **Edit Attribute** button to edit the field. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Use the metadata browser](../customize/create-edit-metadata.md#BKMK_MetadataBrowser). 
  
 All fields have the following properties:  
  
|Property|Description|  
|--------------|-----------------|  
|**Display Name**|The name that appears as a label in the header for lists where this attribute is included. It is also the default label when this field is shown in a form, but the label text in each form can be edited separately.|  
|**Name**|This field is pre-populated based on this **Display Name** you enter. It includes the solution publisher customization prefix. You can change the **Display Name** later, but the **Name** can’t be changed after the field is saved.|  
|**Field Requirement**|There are three options:<br /><br /> - **Optional**<br />     This field doesn’t require data to save the record.<br />- **Business Recommended**<br />     This field doesn’t require data to save the record. However a blue asterisk appears near the field to indicate it is important.<br />- **Business Required**<br />     The record can’t be saved without data in this field.<br />     Be careful when you make fields business required. People will resist using the application if they can’t save records because they lack the correct information to enter into a required field. People may enter incorrect data simply to save the record and get on with their work.<br />     You can use business rules or form scripts to change the requirement level as the data in the record changes as people work on it. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Creating and editing business rules](../customize/create-business-rules-recommendations-apply-logic-form.md)|  
|**Searchable**|When a field is searchable it appears in Advanced Find and is available when customizing views. Use this when there are fields for the entity that you don’t use. Setting this to **No** will reduce the number of options shown to people using advanced find.|  
|**Field Security**|For custom fields, enable this to allow this field to participate in field level security.|  
|**Auditing**|Disable this so that data in this field won’t be included with auditing data.|  
|**Description**|Set text that will appear as a tooltip when the field is displayed in a form. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Video: Dynamics CRM Customizable Tool Tips](http://www.youtube.com/watch?v=7oqtyF6FA8E&list=PLC3591A8FE4ADBE07&index=5)|  
|**Type**|Select the type of record. Depending on the type you select, you’ll have different options. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Types of fields](../customize/types-of-fields.md)|  
  
 Any of the fields that provide direct text input have an **IME Mode**. The input method editor (IME) is used for East Asian languages like Japanese. IMEs allow the user to enter the thousands of different characters used in East Asian written languages using a standard 101-key keyboard.  
  
### Create or edit entity fields  
 Create new fields to capture data when existing system entities don’t have fields that meet your requirements. After you create new fields, be sure to include them on the forms and views for the entity so that they are available from the relevant [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] user interface. You can also add the new fields to reports with the following restrictions:  
  
-   Some system entities or custom entities that are included in a managed solution may not allow you to add new fields.  
  
-   Some system fields or custom fields that are included in a managed solution may not allow you to edit them.  
  
-   The default solution is a special unmanaged solution which shows you all solution components from any managed or unmanaged solutions. You can’t edit ANYTHING in the context of a managed solution. But all the things you find there are in your default solution anyway, so you don’t need to.  
  
1. [!INCLUDE[proc_permissions_system_admin](../includes/proc-permissions-system-admin.md)]  
  
2. [!INCLUDE[proc_settings_customization](../includes/proc-settings-customization.md)]  
  
3.  Click **Customize the System**.  
  
4.  Under **Components**, expand **Entities**, and then expand the entity you want.  
  
5.  Select **Fields**.  
  
    -   To add a new field, on the Actions toolbar, select **New**, and enter a **Display Name** to generate the **Name**.  
  
         \- OR -  
  
    -   To edit one or more fields, select the field or fields (using the Shift key) you want to modify and then on the Actions toolbar, select **Edit**. You can make changes to the following fields:  
  
        -   For **Field Requirement**, select whether it’s optional, recommended, or required.  
  
        -   In **Searchable**, select whether to include this field in the list of fields shown in Advanced Find for this entity and also in the field available for customizing the find columns in the Quick Find view and the Lookup view.  
  
        -   For **Field Security**, enable or disable the feature for this field.  
  
        -   For **Auditing**, enable or disable the feature for this field.  
  
    > [!NOTE]
    >  When you select multiple fields to edit, the **Edit Multiple Fields** dialog appears. You can edit **Field Requirement**, **Searchable**, and **Auditing**.  
  
6.  For new fields, under **Type**, enter the required information for the specified type. For existing fields, you cannot modify the type, but you can modify the settings for the [types of fields](../customize/types-of-fields.md).  
  
7.  Select the **Field type**, **Format**, and **Maximum length** of the field.  
  
8.  Select the **IME mode** for this attribute.  
  
    > [!NOTE]
    >  This specifies whether the active state of an input method editor (IME) is enabled. An IME lets you enter and edit Chinese, Japanese, and Korean characters. IMEs can be in an active or inactive state. The active state accepts Chinese, Japanese, or Korean characters. The inactive state behaves like a regular keyboard and uses a limited set of characters.  
  
9. For a new field, be sure to add a **Description** of the field – this provides instructions to your users on how to use the new field.  
  
10. Click **Save and Close**.  
  
11. Publish your customization.  
  
    -   To publish your changes for one entity, under **Components**, select **Entities**, and then the entity that you made changes to. On the Actions toolbar, select **Publish**.  
  
    -   To publish all changes you have made to multiple entities or components, on the Actions toolbar, select **Publish All Customizations**.  
  
> [!NOTE]
>  Installing a solution or publishing customizations can interfere with normal system operation. We recommend that you schedule a solution publish when it’s least disruptive to users.  

### See also  
 [Entities and metadata overview](../customize/create-edit-metadata.md)   
 [Create and edit entities](../customize/create-edit-entities.md)   
 [Create and edit entity relationships](../customize/create-edit-entity-relationships.md)   
 [Create and edit global option sets](../customize/create-edit-global-option-sets.md)   
 [Edit status reason transitions](../customize/define-status-reason-transitions.md#BKMK_EditStatusReasonTransitions) <br/>
 [Set custom icon for custom case origin](../customer-service/set-custom-icon-custom-case-origin.md)   
 [Define rollup fields](../customize/define-rollup-fields.md)   
 [Define calculated fields](../customize/define-calculated-fields.md)   
 [Behavior and format of the date and time field](../customize/behavior-format-date-time-field.md)   
 