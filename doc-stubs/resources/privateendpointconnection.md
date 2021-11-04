---
title: "privateEndpointConnection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# privateEndpointConnection resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List privateEndpointConnections](../api/privateendpointconnection-list.md)|[privateEndpointConnection](../resources/privateendpointconnection.md) collection|Get a list of the [privateEndpointConnection](../resources/privateendpointconnection.md) objects and their properties.|
|[Create privateEndpointConnection](../api/privatelinkpolicy-post-privateendpointconnections.md)|[privateEndpointConnection](../resources/privateendpointconnection.md)|Create a new [privateEndpointConnection](../resources/privateendpointconnection.md) object.|
|[Get privateEndpointConnection](../api/privateendpointconnection-get.md)|[privateEndpointConnection](../resources/privateendpointconnection.md)|Read the properties and relationships of a [privateEndpointConnection](../resources/privateendpointconnection.md) object.|
|[Update privateEndpointConnection](../api/privateendpointconnection-update.md)|[privateEndpointConnection](../resources/privateendpointconnection.md)|Update the properties of a [privateEndpointConnection](../resources/privateendpointconnection.md) object.|
|[Delete privateEndpointConnection](../api/privateendpointconnection-delete.md)|None|Deletes a [privateEndpointConnection](../resources/privateendpointconnection.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|externalPrivateEndpointId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|privateLinkIds|Int32 collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privateEndpointConnection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privateEndpointConnection",
  "id": "String (identifier)",
  "externalPrivateEndpointId": "String",
  "privateLinkIds": [
    "Integer"
  ]
}
```
