---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewNamedLocation()
displayName := "Untrusted named location with only IPv4 address"
requestBody.SetDisplayName(&displayName) 
additionalData := map[string]interface{}{
	isTrusted := false
requestBody.SetIsTrusted(&isTrusted) 


 := graphmodels.New()
cidrAddress := "6.5.4.3/18"
.SetCidrAddress(&cidrAddress) 

	ipRanges := []graphmodels.Objectable {
		,

	}
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Identity().ConditionalAccess().NamedLocations().ByNamedLocationId("namedLocation-id").Patch(context.Background(), requestBody, nil)


```