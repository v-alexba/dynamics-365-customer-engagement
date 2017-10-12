---
title: "Microsoft Dynamics 365 Customer Engagement adx_redirect EntityType Reference | MicrosoftDocs"
ms.date: 07/10/2017
ms.service: "crm-online"
ms.topic: "reference"
applies_to: 
  - "Dynamics 365 (online)"
ms.assetid: d71742fa-02b4-4b5b-aba8-a70ded211ce1
author: "jimdaly"
ms.author: "jdaly"
manager: "jdaly"
meta-description: "Reference information about the Web API adx_redirect entitytype."
---
# adx_redirect EntityType
<table>
<tr><td><b>Description:</b></td><td>[!INCLUDE[./descriptions/adx_redirect.md](./descriptions/adx_redirect.md)]</td></tr>
<tr><td><b>Entity Set path:</b></td><td>[!include[current-web-api-base-uri.md](../includes/current-web-api-base-uri.md)]adx_redirects </td></tr>
<tr><td><b>Base Type:</b></td><td>[crmbaseentity EntityType](crmbaseentity.md)</td></tr>
<tr><td><b>Display Name:</b></td><td>Redirect</td></tr>
<tr><td><b>Primary Key:</b></td><td>adx_redirectid</td></tr>
<tr><td><b>Primary Name Attribute:</b></td><td>adx_name</td></tr>
<tr><td><b>Operations supported:</b></td><td>POST,GET,PATCH,DELETE</td></tr>
</table>
  
The adx_redirect entitytype has no functions or actions bound to it.

## Properties
Properties represent fields of data stored in the entity. Some properties are read-only. 


|Name|Type|Details|  
|----|----|-------|  
|adx_inboundurl|Edm.String|**Display Name**: Inbound URL<br />**Description**: The path to redirect visitors from<br />|
|adx_name|Edm.String|**Display Name**: Name<br />|
|adx_redirectid|Edm.Guid|**Display Name**: Redirect<br />**Description**: Shows the entity instance.<br />|
|adx_redirecturl|Edm.String|**Display Name**: Redirect URL<br />**Description**: The path to redirect visitors to<br />|
|adx_statuscode|Edm.Int32|**Display Name**: Status Code<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>301</td><td>301 (Permanent Redirect)</td></tr><tr><td>302</td><td>302 (Temporary Redirect)</td></tr><tbody></table>|
|createdon|Edm.DateTimeOffset|**Display Name**: Created On<br />**Description**: Shows the date and time when the record was created.<br />Read-only<br />|
|importsequencenumber|Edm.Int32|**Display Name**: Import Sequence Number<br />**Description**: Shows the sequence number of the import that created this record.<br />|
|modifiedon|Edm.DateTimeOffset|**Display Name**: Modified On<br />**Description**: Shows the date and time when the record was modified.<br />Read-only<br />|
|overriddencreatedon|Edm.DateTimeOffset|**Display Name**: Record Created On<br />**Description**: Shows the date and time that the record was migrated.<br />|
|statecode|Edm.Int32|**Display Name**: Status<br />**Description**: Status of the Redirect<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>0</td><td>Active</td></tr><tr><td>1</td><td>Inactive</td></tr><tbody></table>|
|statuscode|Edm.Int32|**Display Name**: Status Reason<br />**Description**: Select the redirect's status.<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>1</td><td>Active</td></tr><tr><td>2</td><td>Inactive</td></tr><tbody></table>|
|timezoneruleversionnumber|Edm.Int32|**Display Name**: Time Zone Rule Version Number<br />**Description**: For internal use only.<br />|
|utcconversiontimezonecode|Edm.Int32|**Display Name**: UTC Conversion Time Zone Code<br />**Description**: Shows the time zone code that was in use when the record was created.<br />|
|versionnumber|Edm.Int64|**Display Name**: Version Number<br />**Description**: Version Number<br />Read-only<br />|

## Lookup Properties
Lookup properties are read-only, computed properties which contain entity primary key Edm.Guid data for one or more corresponding single-valued navigation properties. More information: [Lookup properties](https://msdn.microsoft.com/library/mt607990.aspx#bkmk_lookupProperties) and [Retrieve data about lookup properties](https://msdn.microsoft.com/library/gg334767.aspx#bkmk_lookupProperty).


|Name|Single-valued navigation property|Description|  
|----|---------------------------------|-----------|  
|_adx_sitemarkerid_value|adx_sitemarkerid<br />|Unique identifier for Site Marker associated with Redirect.|
|_adx_webpageid_value|adx_webpageid<br />|Unique identifier for Web Page associated with Redirect.|
|_adx_websiteid_value|adx_websiteid<br />|Unique identifier for Website associated with Redirect.|
|_createdby_value|createdby<br />|Shows who created the record.|
|_createdonbehalfby_value|createdonbehalfby<br />|Shows who created the record on behalf of another user.|
|_modifiedby_value|modifiedby<br />|Shows who last updated the record.|
|_modifiedonbehalfby_value|modifiedonbehalfby<br />|Shows who last updated the record on behalf of another user.|
|_ownerid_value|ownerid<br />|Enter the user who is assigned to manage the record. This field is updated every time the record is assigned to a different user.|
|_owningbusinessunit_value|owningbusinessunit<br />|Shows the business unit that owns the record.|
|_owningteam_value|owningteam<br />|Unique identifier for the team that owns the record.|
|_owninguser_value|owninguser<br />|Unique identifier for the user that owns the record.|


## Single-valued navigation properties
Single-valued navigation properties represent lookup fields where a single entity can be referenced. Each single-valued navigation property has a corresponding partner collection-valued navigation property on the related entity.


|Name|Type|Partner|  
|----|----|-------|  
|adx_sitemarkerid|[adx_sitemarker EntityType](adx_sitemarker.md)|adx_sitemarker_redirect|
|adx_webpageid|[adx_webpage EntityType](adx_webpage.md)|adx_webpage_redirect|
|adx_websiteid|[adx_website EntityType](adx_website.md)|adx_website_redirect|
|createdby|[systemuser EntityType](systemuser.md)|lk_adx_redirect_createdby|
|createdonbehalfby|[systemuser EntityType](systemuser.md)|lk_adx_redirect_createdonbehalfby|
|modifiedby|[systemuser EntityType](systemuser.md)|lk_adx_redirect_modifiedby|
|modifiedonbehalfby|[systemuser EntityType](systemuser.md)|lk_adx_redirect_modifiedonbehalfby|
|ownerid|[principal EntityType](principal.md)|owner_adx_redirect|
|owningbusinessunit|[businessunit EntityType](businessunit.md)|business_unit_adx_redirect|
|owningteam|[team EntityType](team.md)|team_adx_redirect|
|owninguser|[systemuser EntityType](systemuser.md)|user_adx_redirect|

## Collection-valued navigation properties
Collection-valued navigation properties represent collections of entities which may represent either a one-to-many (1:N) or many-to-many (N:N) relationship between the entities.


|Name|Type|Partner|  
|----|----|-------|  
|adx_redirect_ActivityPointers|[activitypointer EntityType](activitypointer.md)|regardingobjectid_adx_redirect|  
|adx_redirect_adx_alertsubscriptions|[adx_alertsubscription EntityType](adx_alertsubscription.md)|regardingobjectid_adx_redirect_adx_alertsubscription|  
|adx_redirect_adx_inviteredemptions|[adx_inviteredemption EntityType](adx_inviteredemption.md)|regardingobjectid_adx_redirect_adx_inviteredemption|  
|adx_redirect_adx_portalcomments|[adx_portalcomment EntityType](adx_portalcomment.md)|regardingobjectid_adx_redirect_adx_portalcomment|  
|adx_redirect_Annotations|[annotation EntityType](annotation.md)|objectid_adx_redirect|  
|adx_redirect_Appointments|[appointment EntityType](appointment.md)|regardingobjectid_adx_redirect_appointment|  
|adx_redirect_AsyncOperations|[asyncoperation EntityType](asyncoperation.md)|regardingobjectid_adx_redirect|  
|adx_redirect_BulkDeleteFailures|[bulkdeletefailure EntityType](bulkdeletefailure.md)|regardingobjectid_adx_redirect|  
|adx_redirect_DuplicateBaseRecord|[duplicaterecord EntityType](duplicaterecord.md)|baserecordid_adx_redirect|  
|adx_redirect_DuplicateMatchingRecord|[duplicaterecord EntityType](duplicaterecord.md)|duplicaterecordid_adx_redirect|  
|adx_redirect_Emails|[email EntityType](email.md)|regardingobjectid_adx_redirect_email|  
|adx_redirect_Faxes|[fax EntityType](fax.md)|regardingobjectid_adx_redirect_fax|  
|adx_redirect_Letters|[letter EntityType](letter.md)|regardingobjectid_adx_redirect_letter|  
|adx_redirect_msdyn_approvals|[msdyn_approval EntityType](msdyn_approval.md)|regardingobjectid_adx_redirect_msdyn_approval|  
|adx_redirect_msdyn_bookingalerts|[msdyn_bookingalert EntityType](msdyn_bookingalert.md)|regardingobjectid_adx_redirect_msdyn_bookingalert|  
|adx_redirect_msdyn_surveyinvites|[msdyn_surveyinvite EntityType](msdyn_surveyinvite.md)|regardingobjectid_adx_redirect_msdyn_surveyinvite|  
|adx_redirect_PhoneCalls|[phonecall EntityType](phonecall.md)|regardingobjectid_adx_redirect_phonecall|  
|adx_redirect_RecurringAppointmentMasters|[recurringappointmentmaster EntityType](recurringappointmentmaster.md)|regardingobjectid_adx_redirect_recurringappointmentmaster|  
|adx_redirect_ServiceAppointments|[serviceappointment EntityType](serviceappointment.md)|regardingobjectid_adx_redirect_serviceappointment|  
|adx_redirect_SocialActivities|[socialactivity EntityType](socialactivity.md)|regardingobjectid_adx_redirect_socialactivity|  
|adx_redirect_SyncErrors|[syncerror EntityType](syncerror.md)|regardingobjectid_adx_redirect|  
|adx_redirect_Tasks|[task EntityType](task.md)|regardingobjectid_adx_redirect_task|  

## Operations
The following operations can be used with the adx_redirect entity type.


|Name|Binding|Description|  
|----|-------|-----------|  
|[GrantAccess Action](../actions/grantaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/grantaccess.md](../actions/descriptions/grantaccess.md)]|  
|[IsValidStateTransition Function](../functions/isvalidstatetransition.md)|Not Bound|[!INCLUDE[../functions/descriptions/isvalidstatetransition.md](../functions/descriptions/isvalidstatetransition.md)]|  
|[ModifyAccess Action](../actions/modifyaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/modifyaccess.md](../actions/descriptions/modifyaccess.md)]|  
|[RetrievePrincipalAccess Function](../functions/retrieveprincipalaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrieveprincipalaccess.md](../functions/descriptions/retrieveprincipalaccess.md)]|  
|[RetrieveSharedPrincipalsAndAccess Function](../functions/retrievesharedprincipalsandaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrievesharedprincipalsandaccess.md](../functions/descriptions/retrievesharedprincipalsandaccess.md)]|  
|[RevokeAccess Action](../actions/revokeaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/revokeaccess.md](../actions/descriptions/revokeaccess.md)]|  

## Solutions
The following solutions include the adx_redirect entity type.


|Name|Description |  
|----|------------|  
|[Dynamics 365 Portals - Portal Base Solution](../solutions/microsoftcrmportalbase.md)|[!INCLUDE[../solutions/descriptions/microsoftcrmportalbase.md](../solutions/descriptions/microsoftcrmportalbase.md)]|    

[!INCLUDE[./remarks/adx_redirect.md](./remarks/adx_redirect.md)]

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