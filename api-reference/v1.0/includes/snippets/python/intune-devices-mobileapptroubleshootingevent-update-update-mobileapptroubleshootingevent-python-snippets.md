---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = MobileAppTroubleshootingEvent(
	odata_type = "#microsoft.graph.mobileAppTroubleshootingEvent",
)

result = await graph_client.device_management.mobile_app_troubleshooting_events.by_mobile_app_troubleshooting_event_id('mobileAppTroubleshootingEvent-id').patch(request_body)


```