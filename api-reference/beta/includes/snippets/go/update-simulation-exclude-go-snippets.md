---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewSimulation()
id := "2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc"
requestBody.SetId(&id) 
status := graphmodels.EXCLUDED_SIMULATIONSTATUS 
requestBody.SetStatus(&status) 
additionalData := map[string]interface{}{
	"odataEtag" : "\"0100aa9b-0000-0100-0000-6396fa270000\"", 
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Security().AttackSimulation().SimulationsById("simulation-id").Patch(context.Background(), requestBody, nil)


```