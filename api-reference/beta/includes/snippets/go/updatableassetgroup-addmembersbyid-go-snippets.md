---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/Admin/Windows/Updates/UpdatableAssets/Item/MicrosoftGraphWindowsUpdatesAddMembersById"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewAddMembersByIdPostRequestBody()
ids := []string {
	"String",
	"String",
	"String",

}
requestBody.SetIds(ids)
memberEntityType := "#microsoft.graph.windowsUpdates.azureADDevice"
requestBody.SetMemberEntityType(&memberEntityType) 

graphClient.Admin().Windows().Updates().UpdatableAssets().ByUpdatableAssetId("updatableAsset-id").MicrosoftGraphWindowsUpdatesAddMembersById().Post(context.Background(), requestBody, nil)


```