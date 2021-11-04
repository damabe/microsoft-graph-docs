---
title: "Update privateLinkPolicy"
description: "Update the properties of a privateLinkPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update privateLinkPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [privateLinkPolicy](../resources/privatelinkpolicy.md) object.

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
PATCH /privateLinkPolicy
PATCH /policyRoot/privateLinkPolicies/{privateLinkPolicyId}
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
|externalPrivateLinkPolicyId|String|**TODO: Add Description** Required.|
|displayName|String|**TODO: Add Description** Required.|
|allowedTenantIds|String collection|**TODO: Add Description** Optional.|
|allowAllTenants|Boolean|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [privateLinkPolicy](../resources/privatelinkpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_privatelinkpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privateLinkPolicy
Content-Type: application/json
Content-length: 209

{
  "@odata.type": "#microsoft.graph.privateLinkPolicy",
  "externalPrivateLinkPolicyId": "String",
  "displayName": "String",
  "allowedTenantIds": [
    "String"
  ],
  "allowAllTenants": "Boolean"
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
  "@odata.type": "#microsoft.graph.privateLinkPolicy",
  "id": "d30fc1fb-c1fb-d30f-fbc1-0fd3fbc10fd3",
  "externalPrivateLinkPolicyId": "String",
  "displayName": "String",
  "allowedTenantIds": [
    "String"
  ],
  "allowAllTenants": "Boolean"
}
```
