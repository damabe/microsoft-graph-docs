---
title: "List crossTenantAccessPolicyInboundSettings"
description: "Get a list of the crossTenantAccessPolicyInboundSetting objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List crossTenantAccessPolicyInboundSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [crossTenantAccessPolicyInboundSetting](../resources/crosstenantaccesspolicyinboundsetting.md) objects and their properties.

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
GET ** Collection URI for Microsoft.DirectoryServices.crossTenantAccessPolicyInboundSetting not found
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

If successful, this method returns a `200 OK` response code and a collection of [crossTenantAccessPolicyInboundSetting](../resources/crosstenantaccesspolicyinboundsetting.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_crosstenantaccesspolicyinboundsetting"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for Microsoft.DirectoryServices.crossTenantAccessPolicyInboundSetting not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.crossTenantAccessPolicyInboundSetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.crossTenantAccessPolicyInboundSetting",
      "id": "77002118-2118-7700-1821-007718210077",
      "isAccessAllowed": "Boolean",
      "isNativeFederationAllowed": "Boolean",
      "targets": [
        {
          "@odata.type": "microsoft.graph.crossTenantAccessPolicyTarget"
        }
      ],
      "isServiceProviderAllowed": "Boolean",
      "isMfaAccepted": "Boolean",
      "isCompliantDeviceAccepted": "Boolean",
      "isHybridAzureADJoinedDeviceAccepted": "Boolean"
    }
  ]
}
```
