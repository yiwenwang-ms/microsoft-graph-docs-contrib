---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Communications.Calls.Item.Transfer.TransferPostRequestBody
{
	TransferTarget = new InvitationParticipantInfo
	{
		EndpointType = EndpointType.Default,
		Identity = new IdentitySet
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"phone" , new Identity
					{
						OdataType = "#microsoft.graph.identity",
						Id = "+12345678901",
					}
				},
			},
		},
		AdditionalData = new Dictionary<string, object>
		{
			{
				"languageId" , "languageId-value"
			},
			{
				"region" , "region-value"
			},
		},
	},
};
await graphClient.Communications.Calls["{call-id}"].Transfer.PostAsync(requestBody);


```