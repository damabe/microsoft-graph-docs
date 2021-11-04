---
title: "Create attributeSet"
description: "Create a new attributeSet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create attributeSet
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new attributeSet object.

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
POST /directory/attributeSets
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [attributeSet](../resources/attributeset.md) object.

You can specify the following properties when creating an **attributeSet**.

|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description** Optional.|
|maxAttributesPerSet|Int32|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [attributeSet](../resources/attributeset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_attributeset_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/attributeSets
Content-Type: application/json
Content-length: 131

{
  "@odata.type": "#Microsoft.DirectoryServices.attributeSet",
  "description": "String",
  "maxAttributesPerSet": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.attributeSet"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.attributeSet",
  "description": "String",
  "id": "2cfbb7aa-b7aa-2cfb-aab7-fb2caab7fb2c",
  "maxAttributesPerSet": "Integer"
}
```
