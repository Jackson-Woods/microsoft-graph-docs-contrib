---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

query_params = CallRecordItemRequestBuilder.CallRecordItemRequestBuilderGetQueryParameters(
		expand = ["sessions($expand=segments)"],
)

request_configuration = CallRecordItemRequestBuilder.CallRecordItemRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.communications.call_records.by_call_record_id('callRecord-id').get(request_configuration = request_configuration)


```