---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/Me/GetMailTips"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewGetMailTipsPostRequestBody()
emailAddresses := []string {
	"danas@contoso.onmicrosoft.com",
	"fannyd@contoso.onmicrosoft.com",

}
requestBody.SetEmailAddresses(emailAddresses)
mailTipsOptions := graphmodels.AUTOMATICREPLIES, MAILBOXFULLSTATUS_MAILTIPSTYPE 
requestBody.SetMailTipsOptions(&mailTipsOptions) 

result, err := graphClient.Me().GetMailTips().Post(context.Background(), requestBody, nil)


```