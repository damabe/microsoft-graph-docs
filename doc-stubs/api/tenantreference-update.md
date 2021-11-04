---
title: "Update tenantReference"
description: "Update the properties of a tenantReference object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update tenantReference
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [tenantReference](../resources/tenantreference.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /directory/outboundSharedUserProfiles/{outboundSharedUserProfileId}/tenants/{tenantReferenceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|tenantId|String|**TODO: Add Description** Required.|



## Response

If successful, this method returns a `200 OK` response code and an updated [tenantReference](../resources/tenantreference.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_tenantreference"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/outboundSharedUserProfiles/{outboundSharedUserProfileId}/tenants/{tenantReferenceId}
Content-Type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.tenantReference",
  "deletedDateTime": "String (timestamp)",
  "tenantId": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.tenantReference",
  "id": "bc7f83fc-83fc-bc7f-fc83-7fbcfc837fbc",
  "deletedDateTime": "String (timestamp)",
  "tenantId": "String"
}
```
