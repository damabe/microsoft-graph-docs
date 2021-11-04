---
title: "List crossTenantAccessPolicyOutboundSettings"
description: "Get a list of the crossTenantAccessPolicyOutboundSetting objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List crossTenantAccessPolicyOutboundSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [crossTenantAccessPolicyOutboundSetting](../resources/crosstenantaccesspolicyoutboundsetting.md) objects and their properties.

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
GET ** Collection URI for Microsoft.DirectoryServices.crossTenantAccessPolicyOutboundSetting not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [crossTenantAccessPolicyOutboundSetting](../resources/crosstenantaccesspolicyoutboundsetting.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_crosstenantaccesspolicyoutboundsetting"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for Microsoft.DirectoryServices.crossTenantAccessPolicyOutboundSetting not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.crossTenantAccessPolicyOutboundSetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.crossTenantAccessPolicyOutboundSetting",
      "id": "9511f44b-f44b-9511-4bf4-11954bf41195",
      "isAccessAllowed": "Boolean",
      "isNativeFederationAllowed": "Boolean",
      "targets": [
        {
          "@odata.type": "microsoft.graph.crossTenantAccessPolicyTarget"
        }
      ]
    }
  ]
}
```
