---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Attachment
{
	OdataType = "#microsoft.graph.referenceAttachment",
	Name = "Personal pictures",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"sourceUrl" , "https://contoso.com/personal/mario_contoso_net/Documents/Pics"
		},
		{
			"providerType" , "oneDriveConsumer"
		},
		{
			"permission" , "Edit"
		},
		{
			"isFolder" , "True"
		},
	},
};
var result = await graphClient.Me.Events["{event-id}"].Attachments.PostAsync(requestBody);


```