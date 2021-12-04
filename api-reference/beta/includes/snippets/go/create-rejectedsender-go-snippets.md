---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
	"@odata.id": "https://graph.microsoft.com/beta/users/alexd@contoso.com",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
	Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).RejectedSenders().$ref().Post(options)


```