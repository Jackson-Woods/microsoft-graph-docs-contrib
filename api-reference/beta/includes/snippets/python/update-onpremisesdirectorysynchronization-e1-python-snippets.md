---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = OnPremisesDirectorySynchronization(
	configuration = OnPremisesDirectorySynchronizationConfiguration(
		accidental_deletion_prevention = OnPremisesAccidentalDeletionPrevention(
			synchronization_prevention_type = OnPremisesDirectorySynchronizationDeletionPreventionType.EnabledForCount,
			alert_threshold = 500,
		),
		synchronization_interval = "PT30M",
		customer_requested_synchronization_interval = "PT1H",
	),
	features = OnPremisesDirectorySynchronizationFeature(
		group_write_back_enabled = True,
	),
)

result = await graph_client.directory.on_premises_synchronization.by_on_premises_directory_synchronization_id('onPremisesDirectorySynchronization-id').patch(request_body)


```