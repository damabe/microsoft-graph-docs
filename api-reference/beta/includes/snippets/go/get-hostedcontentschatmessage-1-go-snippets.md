---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
chatMessageId := "chatMessage-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).HostedContents().Get(nil)


```