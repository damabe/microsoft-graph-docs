---
title: "Update crossTenantAccessPolicyInboundSetting"
description: "Update the properties of a crossTenantAccessPolicyInboundSetting object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update crossTenantAccessPolicyInboundSetting
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [crossTenantAccessPolicyInboundSetting](../resources/crosstenantaccesspolicyinboundsetting.md) object.

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
PATCH /crossTenantAccessPolicyInboundSetting
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
|isAccessAllowed|Boolean|**TODO: Add Description** Inherited from [crossTenantAccessPolicySettingsBase](../resources/crosstenantaccesspolicysettingsbase.md). Optional.|
|isNativeFederationAllowed|Boolean|**TODO: Add Description** Inherited from [crossTenantAccessPolicySettingsBase](../resources/crosstenantaccesspolicysettingsbase.md). Optional.|
|targets|[Microsoft.DirectoryServices.crossTenantAccessPolicyTarget](../resources/crosstenantaccesspolicytarget.md) collection|**TODO: Add Description** Inherited from [crossTenantAccessPolicySettingsBase](../resources/crosstenantaccesspolicysettingsbase.md). Optional.|
|isServiceProviderAllowed|Boolean|**TODO: Add Description** Optional.|
|isMfaAccepted|Boolean|**TODO: Add Description** Optional.|
|isCompliantDeviceAccepted|Boolean|**TODO: Add Description** Optional.|
|isHybridAzureADJoinedDeviceAccepted|Boolean|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [crossTenantAccessPolicyInboundSetting](../resources/crosstenantaccesspolicyinboundsetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_crosstenantaccesspolicyinboundsetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/crossTenantAccessPolicyInboundSetting
Content-Type: application/json
Content-length: 430

{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyInboundSetting",
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
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyInboundSetting",
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
```
