---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.DirectoryNamespace.DeletedItems.Item.DeletedItem
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"userId" , "55ac777c-109e-4022-b58c-470c8fcb6892"
		},
		{
			"type" , "Group"
		},
	},
};
await graphClient.Directory.DeletedItems["{directoryObject-id}"].PostAsync(requestBody);


```