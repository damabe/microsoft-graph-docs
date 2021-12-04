---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetIds( []String {
	"80a963dd-84af-4eb8-b2a6-781e444d4fb0",
	"62e90394-69f5-4237-9190-012177145e10",
	"86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
	"ac38546e-ddf3-437a-ac5c-27a94cd7a0f1",
}
options := &msgraphsdk.CheckMemberObjectsRequestBuilderPostOptions{
	Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).CheckMemberObjects().Post(options)


```