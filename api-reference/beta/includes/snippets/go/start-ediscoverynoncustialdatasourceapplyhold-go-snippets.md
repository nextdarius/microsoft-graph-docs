---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/Security/Cases/EdiscoveryCases/Item/NoncustodialDataSources/MicrosoftGraphSecurityApplyHold"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewApplyHoldPostRequestBody()
ids := []string {
	"39333641443238353535383731453339",
	"46333131344239353834433430454335",

}
requestBody.SetIds(ids)

graphClient.Security().Cases().EdiscoveryCases().ByEdiscoveryCaseId("ediscoveryCase-id").NoncustodialDataSources().MicrosoftGraphSecurityApplyHold().Post(context.Background(), requestBody, nil)


```