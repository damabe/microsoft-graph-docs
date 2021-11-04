---
title: "List organizationalBrandingProperties"
description: "Get a list of the organizationalBrandingProperties objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List organizationalBrandingProperties
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) objects and their properties.

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
GET ** Collection URI for Microsoft.DirectoryServices.organizationalBrandingProperties not found
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

If successful, this method returns a `200 OK` response code and a collection of [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_organizationalbrandingproperties"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for Microsoft.DirectoryServices.organizationalBrandingProperties not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.organizationalBrandingProperties)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.organizationalBrandingProperties",
      "id": "9816068c-068c-9816-8c06-16988c061698",
      "backgroundColor": "String",
      "backgroundImage": "Stream",
      "backgroundImageRelativeUrl": "String",
      "bannerLogo": "Stream",
      "bannerLogoRelativeUrl": "String",
      "cdnList": [
        "String"
      ],
      "signInPageText": "String",
      "squareDarkLogo": "Stream",
      "squareDarkLogoRelativeUrl": "String",
      "squareLogo": "Stream",
      "squareLogoRelativeUrl": "String",
      "usernameHintText": "String",
      "customAccountResetCredentialsUrl": "String",
      "customCannotAccessYourAccountText": "String",
      "customCannotAccessYourAccountUrl": "String",
      "customForgotMyPasswordText": "String",
      "customPrivacyAndCookiesText": "String",
      "customPrivacyAndCookiesUrl": "String",
      "customResetItNowText": "String",
      "customTermsOfUseText": "String",
      "customTermsOfUseUrl": "String",
      "favicon": "Stream",
      "faviconRelativeUrl": "String",
      "headerBackgroundColor": "String",
      "loginPageTextVisibilitySettings": {
        "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
      }
    }
  ]
}
```
