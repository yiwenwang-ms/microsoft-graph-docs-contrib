---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new MobileAppTroubleshootingEvent
{
	OdataType = "#microsoft.graph.mobileAppTroubleshootingEvent",
};
var result = await graphClient.DeviceManagement.MobileAppTroubleshootingEvents.PostAsync(requestBody);


```